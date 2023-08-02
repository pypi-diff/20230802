# Comparing `tmp/types-aiobotocore-lexv2-models-2.5.2.tar.gz` & `tmp/types-aiobotocore-lexv2-models-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lexv2-models-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-lexv2-models-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-lexv2-models-2.5.2.tar` & `types-aiobotocore-lexv2-models-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.402428 types-aiobotocore-lexv2-models-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30280 2023-07-08 01:43:53.402428 types-aiobotocore-lexv2-models-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.402428 types-aiobotocore-lexv2-models-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.402428 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69471 2023-07-08 01:33:56.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69369 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-07-08 01:33:56.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-07-08 01:33:56.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   150439 2023-07-08 01:34:00.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   150242 2023-07-08 01:33:57.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:55.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-07-08 01:33:56.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-08 01:33:56.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.402428 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30280 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32581 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:42:03.000000 types-aiobotocore-lexv2-models-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.645542 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69636 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69534 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174293 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174061 2023-08-02 14:42:06.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32581 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/LICENSE` & `types-aiobotocore-lexv2-models-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/PKG-INFO` & `types-aiobotocore-lexv2-models-2.5.2.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lexv2-models
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexModelsV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexModelsV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lexv2-models type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lexv2-models type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-models"></a>
 
 # types-aiobotocore-lexv2-models
 
 [![PyPI - types-aiobotocore-lexv2-models](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lexv2-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lexv2-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-models)](https://pepy.tech/project/types-aiobotocore-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexModelsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [types-aiobotocore-lexv2-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +73,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -403,20 +402,20 @@
 )
 
 
 def check_value(value: AggregatedUtterancesFilterNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lexv2_models.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lexv2_models.type_defs import (
     ActiveContextTypeDef,
     AdvancedRecognitionSettingTypeDef,
     ExecutionErrorDetailsTypeDef,
     AgentTurnSpecificationTypeDef,
@@ -428,14 +427,15 @@
     AssociatedTranscriptTypeDef,
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
     CustomVocabularyItemTypeDef,
     FailedCustomVocabularyItemTypeDef,
+    ResponseMetadataTypeDef,
     CustomVocabularyEntryIdTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
     BotAliasTestExecutionTargetTypeDef,
     BotExportSpecificationTypeDef,
     BotFilterTypeDef,
     DataPrivacyTypeDef,
@@ -451,101 +451,86 @@
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
-    BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
     ButtonTypeDef,
     CloudWatchLogGroupLogDestinationTypeDef,
     LambdaCodeHookTypeDef,
     SubSlotTypeCompositionTypeDef,
     ConditionTypeDef,
     ConversationLevelIntentClassificationResultItemTypeDef,
     ConversationLevelResultDetailTypeDef,
     ConversationLevelSlotResolutionResultItemTypeDef,
     ConversationLevelTestResultsFilterByTypeDef,
-    ConversationLogsDataSourceFilterByTypeDef,
+    ConversationLogsDataSourceFilterByOutputTypeDef,
+    TimestampTypeDef,
     SentimentAnalysisSettingsTypeDef,
     DialogCodeHookSettingsTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     SampleUtteranceTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
-    CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
-    CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
-    CreateUploadUrlResponseTypeDef,
     CustomPayloadTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
-    DateRangeFilterTypeDef,
+    DateRangeFilterOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
-    DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
-    DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
-    DeleteBotResponseTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
-    DeleteBotVersionResponseTypeDef,
     DeleteCustomVocabularyRequestRequestTypeDef,
-    DeleteCustomVocabularyResponseTypeDef,
     DeleteExportRequestRequestTypeDef,
-    DeleteExportResponseTypeDef,
     DeleteImportRequestRequestTypeDef,
-    DeleteImportResponseTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
-    DeleteResourcePolicyStatementResponseTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
-    DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
     SlotPriorityTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
     TestSetStorageLocationTypeDef,
     DescribeTestSetRequestRequestTypeDef,
     DialogActionTypeDef,
+    IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportFilterTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
-    GetTestExecutionArtifactsUrlResponseTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
     IntentFilterTypeDef,
@@ -557,60 +542,78 @@
     RecommendedIntentSummaryTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
     PlainTextMessageTypeDef,
     SSMLMessageTypeDef,
     OverallTestResultItemTypeDef,
+    PathFormatOutputTypeDef,
     PathFormatTypeDef,
     TextInputSpecificationTypeDef,
     RelativeAggregationDurationTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     SampleValueTypeDef,
     SlotDefaultValueTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
     SlotValueTypeDef,
     SlotValueRegexFilterTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
-    StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
-    UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
-    SearchAssociatedTranscriptsResponseTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
     BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
-    ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
+    BuildBotLocaleResponseTypeDef,
+    CreateResourcePolicyResponseTypeDef,
+    CreateResourcePolicyStatementResponseTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    DeleteBotAliasResponseTypeDef,
+    DeleteBotLocaleResponseTypeDef,
+    DeleteBotResponseTypeDef,
+    DeleteBotVersionResponseTypeDef,
+    DeleteCustomVocabularyResponseTypeDef,
+    DeleteExportResponseTypeDef,
+    DeleteImportResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyStatementResponseTypeDef,
+    DescribeCustomVocabularyMetadataResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetTestExecutionArtifactsUrlResponseTypeDef,
+    ListCustomVocabularyItemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SearchAssociatedTranscriptsResponseTypeDef,
+    StopBotRecommendationResponseTypeDef,
+    UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     TestExecutionTargetTypeDef,
+    BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
     BotLocaleImportSpecificationTypeDef,
     CreateBotLocaleRequestRequestTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
     UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
@@ -629,37 +632,42 @@
     CreateBotVersionResponseTypeDef,
     ListBotVersionsRequestRequestTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsRequestRequestTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesRequestRequestTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
     TextLogDestinationTypeDef,
     CodeHookSpecificationTypeDef,
+    CompositeSlotTypeSettingOutputTypeDef,
     CompositeSlotTypeSettingTypeDef,
     ConversationLevelTestResultItemTypeDef,
     TestExecutionResultFilterByTypeDef,
-    ConversationLogsDataSourceTypeDef,
+    ConversationLogsDataSourceOutputTypeDef,
+    ConversationLogsDataSourceFilterByTypeDef,
+    DateRangeFilterTypeDef,
     IntentSummaryTypeDef,
     CreateResourcePolicyStatementRequestRequestTypeDef,
-    LexTranscriptFilterTypeDef,
+    LexTranscriptFilterOutputTypeDef,
     DescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
     DescribeBotVersionResponseTypeDef,
     UpdateBotRecommendationRequestRequestTypeDef,
     DescribeTestSetResponseTypeDef,
     TestSetSummaryTypeDef,
     UpdateTestSetResponseTypeDef,
+    DialogStateOutputTypeDef,
     DialogStateTypeDef,
     ExportResourceSpecificationTypeDef,
     ListExportsRequestRequestTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     InputSessionStateSpecificationTypeDef,
@@ -670,130 +678,178 @@
     ListSlotTypesResponseTypeDef,
     ListSlotsRequestRequestTypeDef,
     ListTestExecutionsRequestRequestTypeDef,
     ListTestSetsRequestRequestTypeDef,
     OverallTestResultsTypeDef,
     UtteranceAggregationDurationTypeDef,
     RuntimeHintDetailsTypeDef,
+    SlotTypeValueOutputTypeDef,
     SlotTypeValueTypeDef,
+    SlotDefaultValueSpecificationOutputTypeDef,
     SlotDefaultValueSpecificationTypeDef,
     SlotResolutionTestResultItemTypeDef,
+    SlotValueOverrideOutputTypeDef,
     SlotValueOverrideTypeDef,
     SlotValueSelectionSettingTypeDef,
     TestSetDiscrepancyErrorsTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
+    TestSetImportResourceSpecificationOutputTypeDef,
     TestSetImportResourceSpecificationTypeDef,
     UserTurnOutputSpecificationTypeDef,
     UtteranceInputSpecificationTypeDef,
     PromptAttemptSpecificationTypeDef,
     AudioLogSettingTypeDef,
     DescribeTestExecutionResponseTypeDef,
     StartTestExecutionRequestRequestTypeDef,
     StartTestExecutionResponseTypeDef,
     TestExecutionSummaryTypeDef,
     BotRecommendationResultsTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     TextLogSettingTypeDef,
     BotAliasLocaleSettingsTypeDef,
+    CompositeSlotTypeSettingUnionTypeDef,
     ConversationLevelTestResultsTypeDef,
     ListTestExecutionResultItemsRequestRequestTypeDef,
-    TestSetGenerationDataSourceTypeDef,
+    TestSetGenerationDataSourceOutputTypeDef,
+    ConversationLogsDataSourceTypeDef,
+    LexTranscriptFilterTypeDef,
     ListIntentsResponseTypeDef,
-    TranscriptFilterTypeDef,
+    TranscriptFilterOutputTypeDef,
     ListTestSetsResponseTypeDef,
     CreateExportRequestRequestTypeDef,
     CreateExportResponseTypeDef,
     DescribeExportResponseTypeDef,
     ExportSummaryTypeDef,
     UpdateExportResponseTypeDef,
     ExternalSourceSettingTypeDef,
     IntentClassificationTestResultsTypeDef,
     ListAggregatedUtterancesRequestRequestTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
+    SlotTypeValueUnionTypeDef,
     IntentLevelSlotResolutionTestResultItemTypeDef,
     CreateTestSetDiscrepancyReportRequestRequestTypeDef,
     CreateTestSetDiscrepancyReportResponseTypeDef,
     DescribeTestSetDiscrepancyReportResponseTypeDef,
+    ImportResourceSpecificationOutputTypeDef,
     ImportResourceSpecificationTypeDef,
     UserTurnInputSpecificationTypeDef,
     ListTestExecutionsResponseTypeDef,
+    MessageGroupOutputTypeDef,
     MessageGroupTypeDef,
+    ConversationLogSettingsOutputTypeDef,
     ConversationLogSettingsTypeDef,
     DescribeTestSetGenerationResponseTypeDef,
-    StartTestSetGenerationRequestRequestTypeDef,
     StartTestSetGenerationResponseTypeDef,
-    S3BucketTranscriptSourceTypeDef,
+    TestSetGenerationDataSourceTypeDef,
+    TranscriptFilterTypeDef,
+    S3BucketTranscriptSourceOutputTypeDef,
     ListExportsResponseTypeDef,
-    CreateSlotTypeRequestRequestTypeDef,
     CreateSlotTypeResponseTypeDef,
     DescribeSlotTypeResponseTypeDef,
-    UpdateSlotTypeRequestRequestTypeDef,
     UpdateSlotTypeResponseTypeDef,
+    CreateSlotTypeRequestRequestTypeDef,
+    UpdateSlotTypeRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultsTypeDef,
     DescribeImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    ImportResourceSpecificationUnionTypeDef,
+    StartImportRequestRequestTypeDef,
     UserTurnResultTypeDef,
     UserTurnSpecificationTypeDef,
+    FulfillmentStartResponseSpecificationOutputTypeDef,
+    FulfillmentUpdateResponseSpecificationOutputTypeDef,
+    PromptSpecificationOutputTypeDef,
+    ResponseSpecificationOutputTypeDef,
+    StillWaitingResponseSpecificationOutputTypeDef,
     FulfillmentStartResponseSpecificationTypeDef,
     FulfillmentUpdateResponseSpecificationTypeDef,
     PromptSpecificationTypeDef,
     ResponseSpecificationTypeDef,
     StillWaitingResponseSpecificationTypeDef,
-    CreateBotAliasRequestRequestTypeDef,
     CreateBotAliasResponseTypeDef,
     DescribeBotAliasResponseTypeDef,
-    UpdateBotAliasRequestRequestTypeDef,
     UpdateBotAliasResponseTypeDef,
-    TranscriptSourceSettingTypeDef,
+    ConversationLogSettingsUnionTypeDef,
+    CreateBotAliasRequestRequestTypeDef,
+    UpdateBotAliasRequestRequestTypeDef,
+    StartTestSetGenerationRequestRequestTypeDef,
+    TestSetGenerationDataSourceUnionTypeDef,
+    S3BucketTranscriptSourceTypeDef,
+    TranscriptSourceSettingOutputTypeDef,
     TestSetTurnResultTypeDef,
     TurnSpecificationTypeDef,
-    FulfillmentUpdatesSpecificationTypeDef,
+    FulfillmentUpdatesSpecificationOutputTypeDef,
     SlotSummaryTypeDef,
+    ConditionalBranchOutputTypeDef,
+    DefaultConditionalBranchOutputTypeDef,
+    WaitAndContinueSpecificationOutputTypeDef,
+    FulfillmentUpdatesSpecificationTypeDef,
     ConditionalBranchTypeDef,
     DefaultConditionalBranchTypeDef,
     WaitAndContinueSpecificationTypeDef,
+    TranscriptSourceSettingTypeDef,
     DescribeBotRecommendationResponseTypeDef,
-    StartBotRecommendationRequestRequestTypeDef,
     StartBotRecommendationResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UtteranceLevelTestResultItemTypeDef,
     TestSetTurnRecordTypeDef,
     ListSlotsResponseTypeDef,
+    ConditionalSpecificationOutputTypeDef,
+    SubSlotValueElicitationSettingOutputTypeDef,
     ConditionalSpecificationTypeDef,
     SubSlotValueElicitationSettingTypeDef,
+    StartBotRecommendationRequestRequestTypeDef,
+    TranscriptSourceSettingUnionTypeDef,
     UtteranceLevelTestResultsTypeDef,
     ListTestSetRecordsResponseTypeDef,
+    IntentClosingSettingOutputTypeDef,
+    PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    PostFulfillmentStatusSpecificationOutputTypeDef,
+    SpecificationsOutputTypeDef,
     IntentClosingSettingTypeDef,
     PostDialogCodeHookInvocationSpecificationTypeDef,
     PostFulfillmentStatusSpecificationTypeDef,
     SpecificationsTypeDef,
     TestExecutionResultItemsTypeDef,
+    DialogCodeHookInvocationSettingOutputTypeDef,
+    FulfillmentCodeHookSettingsOutputTypeDef,
+    SubSlotSettingOutputTypeDef,
+    IntentClosingSettingUnionTypeDef,
     DialogCodeHookInvocationSettingTypeDef,
     FulfillmentCodeHookSettingsTypeDef,
     SubSlotSettingTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
+    InitialResponseSettingOutputTypeDef,
+    IntentConfirmationSettingOutputTypeDef,
+    SlotCaptureSettingOutputTypeDef,
     InitialResponseSettingTypeDef,
     IntentConfirmationSettingTypeDef,
     SlotCaptureSettingTypeDef,
-    CreateIntentRequestRequestTypeDef,
+    FulfillmentCodeHookSettingsUnionTypeDef,
+    SubSlotSettingUnionTypeDef,
     CreateIntentResponseTypeDef,
     DescribeIntentResponseTypeDef,
-    UpdateIntentRequestRequestTypeDef,
     UpdateIntentResponseTypeDef,
+    SlotValueElicitationSettingOutputTypeDef,
+    InitialResponseSettingUnionTypeDef,
+    CreateIntentRequestRequestTypeDef,
+    IntentConfirmationSettingUnionTypeDef,
+    UpdateIntentRequestRequestTypeDef,
     SlotValueElicitationSettingTypeDef,
-    CreateSlotRequestRequestTypeDef,
     CreateSlotResponseTypeDef,
     DescribeSlotResponseTypeDef,
-    UpdateSlotRequestRequestTypeDef,
     UpdateSlotResponseTypeDef,
+    CreateSlotRequestRequestTypeDef,
+    SlotValueElicitationSettingUnionTypeDef,
+    UpdateSlotRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTypeDef:
+def get_value() -> ActiveContextTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/README.md` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-lexv2-models
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexModelsV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore lexv2-models type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-models"></a>
 
 # types-aiobotocore-lexv2-models
 
 [![PyPI - types-aiobotocore-lexv2-models](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lexv2-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lexv2-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-models)](https://pepy.tech/project/types-aiobotocore-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexModelsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [types-aiobotocore-lexv2-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -370,20 +402,20 @@
 )
 
 
 def check_value(value: AggregatedUtterancesFilterNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lexv2_models.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lexv2_models.type_defs import (
     ActiveContextTypeDef,
     AdvancedRecognitionSettingTypeDef,
     ExecutionErrorDetailsTypeDef,
     AgentTurnSpecificationTypeDef,
@@ -395,14 +427,15 @@
     AssociatedTranscriptTypeDef,
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
     CustomVocabularyItemTypeDef,
     FailedCustomVocabularyItemTypeDef,
+    ResponseMetadataTypeDef,
     CustomVocabularyEntryIdTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
     BotAliasTestExecutionTargetTypeDef,
     BotExportSpecificationTypeDef,
     BotFilterTypeDef,
     DataPrivacyTypeDef,
@@ -418,101 +451,86 @@
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
-    BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
     ButtonTypeDef,
     CloudWatchLogGroupLogDestinationTypeDef,
     LambdaCodeHookTypeDef,
     SubSlotTypeCompositionTypeDef,
     ConditionTypeDef,
     ConversationLevelIntentClassificationResultItemTypeDef,
     ConversationLevelResultDetailTypeDef,
     ConversationLevelSlotResolutionResultItemTypeDef,
     ConversationLevelTestResultsFilterByTypeDef,
-    ConversationLogsDataSourceFilterByTypeDef,
+    ConversationLogsDataSourceFilterByOutputTypeDef,
+    TimestampTypeDef,
     SentimentAnalysisSettingsTypeDef,
     DialogCodeHookSettingsTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     SampleUtteranceTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
-    CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
-    CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
-    CreateUploadUrlResponseTypeDef,
     CustomPayloadTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
-    DateRangeFilterTypeDef,
+    DateRangeFilterOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
-    DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
-    DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
-    DeleteBotResponseTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
-    DeleteBotVersionResponseTypeDef,
     DeleteCustomVocabularyRequestRequestTypeDef,
-    DeleteCustomVocabularyResponseTypeDef,
     DeleteExportRequestRequestTypeDef,
-    DeleteExportResponseTypeDef,
     DeleteImportRequestRequestTypeDef,
-    DeleteImportResponseTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
-    DeleteResourcePolicyStatementResponseTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
-    DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
     SlotPriorityTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
     TestSetStorageLocationTypeDef,
     DescribeTestSetRequestRequestTypeDef,
     DialogActionTypeDef,
+    IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportFilterTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
-    GetTestExecutionArtifactsUrlResponseTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
     IntentFilterTypeDef,
@@ -524,60 +542,78 @@
     RecommendedIntentSummaryTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
     PlainTextMessageTypeDef,
     SSMLMessageTypeDef,
     OverallTestResultItemTypeDef,
+    PathFormatOutputTypeDef,
     PathFormatTypeDef,
     TextInputSpecificationTypeDef,
     RelativeAggregationDurationTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     SampleValueTypeDef,
     SlotDefaultValueTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
     SlotValueTypeDef,
     SlotValueRegexFilterTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
-    StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
-    UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
-    SearchAssociatedTranscriptsResponseTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
     BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
-    ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
+    BuildBotLocaleResponseTypeDef,
+    CreateResourcePolicyResponseTypeDef,
+    CreateResourcePolicyStatementResponseTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    DeleteBotAliasResponseTypeDef,
+    DeleteBotLocaleResponseTypeDef,
+    DeleteBotResponseTypeDef,
+    DeleteBotVersionResponseTypeDef,
+    DeleteCustomVocabularyResponseTypeDef,
+    DeleteExportResponseTypeDef,
+    DeleteImportResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyStatementResponseTypeDef,
+    DescribeCustomVocabularyMetadataResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetTestExecutionArtifactsUrlResponseTypeDef,
+    ListCustomVocabularyItemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SearchAssociatedTranscriptsResponseTypeDef,
+    StopBotRecommendationResponseTypeDef,
+    UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     TestExecutionTargetTypeDef,
+    BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
     BotLocaleImportSpecificationTypeDef,
     CreateBotLocaleRequestRequestTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
     UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
@@ -596,37 +632,42 @@
     CreateBotVersionResponseTypeDef,
     ListBotVersionsRequestRequestTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsRequestRequestTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesRequestRequestTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
     TextLogDestinationTypeDef,
     CodeHookSpecificationTypeDef,
+    CompositeSlotTypeSettingOutputTypeDef,
     CompositeSlotTypeSettingTypeDef,
     ConversationLevelTestResultItemTypeDef,
     TestExecutionResultFilterByTypeDef,
-    ConversationLogsDataSourceTypeDef,
+    ConversationLogsDataSourceOutputTypeDef,
+    ConversationLogsDataSourceFilterByTypeDef,
+    DateRangeFilterTypeDef,
     IntentSummaryTypeDef,
     CreateResourcePolicyStatementRequestRequestTypeDef,
-    LexTranscriptFilterTypeDef,
+    LexTranscriptFilterOutputTypeDef,
     DescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
     DescribeBotVersionResponseTypeDef,
     UpdateBotRecommendationRequestRequestTypeDef,
     DescribeTestSetResponseTypeDef,
     TestSetSummaryTypeDef,
     UpdateTestSetResponseTypeDef,
+    DialogStateOutputTypeDef,
     DialogStateTypeDef,
     ExportResourceSpecificationTypeDef,
     ListExportsRequestRequestTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     InputSessionStateSpecificationTypeDef,
@@ -637,130 +678,178 @@
     ListSlotTypesResponseTypeDef,
     ListSlotsRequestRequestTypeDef,
     ListTestExecutionsRequestRequestTypeDef,
     ListTestSetsRequestRequestTypeDef,
     OverallTestResultsTypeDef,
     UtteranceAggregationDurationTypeDef,
     RuntimeHintDetailsTypeDef,
+    SlotTypeValueOutputTypeDef,
     SlotTypeValueTypeDef,
+    SlotDefaultValueSpecificationOutputTypeDef,
     SlotDefaultValueSpecificationTypeDef,
     SlotResolutionTestResultItemTypeDef,
+    SlotValueOverrideOutputTypeDef,
     SlotValueOverrideTypeDef,
     SlotValueSelectionSettingTypeDef,
     TestSetDiscrepancyErrorsTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
+    TestSetImportResourceSpecificationOutputTypeDef,
     TestSetImportResourceSpecificationTypeDef,
     UserTurnOutputSpecificationTypeDef,
     UtteranceInputSpecificationTypeDef,
     PromptAttemptSpecificationTypeDef,
     AudioLogSettingTypeDef,
     DescribeTestExecutionResponseTypeDef,
     StartTestExecutionRequestRequestTypeDef,
     StartTestExecutionResponseTypeDef,
     TestExecutionSummaryTypeDef,
     BotRecommendationResultsTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     TextLogSettingTypeDef,
     BotAliasLocaleSettingsTypeDef,
+    CompositeSlotTypeSettingUnionTypeDef,
     ConversationLevelTestResultsTypeDef,
     ListTestExecutionResultItemsRequestRequestTypeDef,
-    TestSetGenerationDataSourceTypeDef,
+    TestSetGenerationDataSourceOutputTypeDef,
+    ConversationLogsDataSourceTypeDef,
+    LexTranscriptFilterTypeDef,
     ListIntentsResponseTypeDef,
-    TranscriptFilterTypeDef,
+    TranscriptFilterOutputTypeDef,
     ListTestSetsResponseTypeDef,
     CreateExportRequestRequestTypeDef,
     CreateExportResponseTypeDef,
     DescribeExportResponseTypeDef,
     ExportSummaryTypeDef,
     UpdateExportResponseTypeDef,
     ExternalSourceSettingTypeDef,
     IntentClassificationTestResultsTypeDef,
     ListAggregatedUtterancesRequestRequestTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
+    SlotTypeValueUnionTypeDef,
     IntentLevelSlotResolutionTestResultItemTypeDef,
     CreateTestSetDiscrepancyReportRequestRequestTypeDef,
     CreateTestSetDiscrepancyReportResponseTypeDef,
     DescribeTestSetDiscrepancyReportResponseTypeDef,
+    ImportResourceSpecificationOutputTypeDef,
     ImportResourceSpecificationTypeDef,
     UserTurnInputSpecificationTypeDef,
     ListTestExecutionsResponseTypeDef,
+    MessageGroupOutputTypeDef,
     MessageGroupTypeDef,
+    ConversationLogSettingsOutputTypeDef,
     ConversationLogSettingsTypeDef,
     DescribeTestSetGenerationResponseTypeDef,
-    StartTestSetGenerationRequestRequestTypeDef,
     StartTestSetGenerationResponseTypeDef,
-    S3BucketTranscriptSourceTypeDef,
+    TestSetGenerationDataSourceTypeDef,
+    TranscriptFilterTypeDef,
+    S3BucketTranscriptSourceOutputTypeDef,
     ListExportsResponseTypeDef,
-    CreateSlotTypeRequestRequestTypeDef,
     CreateSlotTypeResponseTypeDef,
     DescribeSlotTypeResponseTypeDef,
-    UpdateSlotTypeRequestRequestTypeDef,
     UpdateSlotTypeResponseTypeDef,
+    CreateSlotTypeRequestRequestTypeDef,
+    UpdateSlotTypeRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultsTypeDef,
     DescribeImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    ImportResourceSpecificationUnionTypeDef,
+    StartImportRequestRequestTypeDef,
     UserTurnResultTypeDef,
     UserTurnSpecificationTypeDef,
+    FulfillmentStartResponseSpecificationOutputTypeDef,
+    FulfillmentUpdateResponseSpecificationOutputTypeDef,
+    PromptSpecificationOutputTypeDef,
+    ResponseSpecificationOutputTypeDef,
+    StillWaitingResponseSpecificationOutputTypeDef,
     FulfillmentStartResponseSpecificationTypeDef,
     FulfillmentUpdateResponseSpecificationTypeDef,
     PromptSpecificationTypeDef,
     ResponseSpecificationTypeDef,
     StillWaitingResponseSpecificationTypeDef,
-    CreateBotAliasRequestRequestTypeDef,
     CreateBotAliasResponseTypeDef,
     DescribeBotAliasResponseTypeDef,
-    UpdateBotAliasRequestRequestTypeDef,
     UpdateBotAliasResponseTypeDef,
-    TranscriptSourceSettingTypeDef,
+    ConversationLogSettingsUnionTypeDef,
+    CreateBotAliasRequestRequestTypeDef,
+    UpdateBotAliasRequestRequestTypeDef,
+    StartTestSetGenerationRequestRequestTypeDef,
+    TestSetGenerationDataSourceUnionTypeDef,
+    S3BucketTranscriptSourceTypeDef,
+    TranscriptSourceSettingOutputTypeDef,
     TestSetTurnResultTypeDef,
     TurnSpecificationTypeDef,
-    FulfillmentUpdatesSpecificationTypeDef,
+    FulfillmentUpdatesSpecificationOutputTypeDef,
     SlotSummaryTypeDef,
+    ConditionalBranchOutputTypeDef,
+    DefaultConditionalBranchOutputTypeDef,
+    WaitAndContinueSpecificationOutputTypeDef,
+    FulfillmentUpdatesSpecificationTypeDef,
     ConditionalBranchTypeDef,
     DefaultConditionalBranchTypeDef,
     WaitAndContinueSpecificationTypeDef,
+    TranscriptSourceSettingTypeDef,
     DescribeBotRecommendationResponseTypeDef,
-    StartBotRecommendationRequestRequestTypeDef,
     StartBotRecommendationResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UtteranceLevelTestResultItemTypeDef,
     TestSetTurnRecordTypeDef,
     ListSlotsResponseTypeDef,
+    ConditionalSpecificationOutputTypeDef,
+    SubSlotValueElicitationSettingOutputTypeDef,
     ConditionalSpecificationTypeDef,
     SubSlotValueElicitationSettingTypeDef,
+    StartBotRecommendationRequestRequestTypeDef,
+    TranscriptSourceSettingUnionTypeDef,
     UtteranceLevelTestResultsTypeDef,
     ListTestSetRecordsResponseTypeDef,
+    IntentClosingSettingOutputTypeDef,
+    PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    PostFulfillmentStatusSpecificationOutputTypeDef,
+    SpecificationsOutputTypeDef,
     IntentClosingSettingTypeDef,
     PostDialogCodeHookInvocationSpecificationTypeDef,
     PostFulfillmentStatusSpecificationTypeDef,
     SpecificationsTypeDef,
     TestExecutionResultItemsTypeDef,
+    DialogCodeHookInvocationSettingOutputTypeDef,
+    FulfillmentCodeHookSettingsOutputTypeDef,
+    SubSlotSettingOutputTypeDef,
+    IntentClosingSettingUnionTypeDef,
     DialogCodeHookInvocationSettingTypeDef,
     FulfillmentCodeHookSettingsTypeDef,
     SubSlotSettingTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
+    InitialResponseSettingOutputTypeDef,
+    IntentConfirmationSettingOutputTypeDef,
+    SlotCaptureSettingOutputTypeDef,
     InitialResponseSettingTypeDef,
     IntentConfirmationSettingTypeDef,
     SlotCaptureSettingTypeDef,
-    CreateIntentRequestRequestTypeDef,
+    FulfillmentCodeHookSettingsUnionTypeDef,
+    SubSlotSettingUnionTypeDef,
     CreateIntentResponseTypeDef,
     DescribeIntentResponseTypeDef,
-    UpdateIntentRequestRequestTypeDef,
     UpdateIntentResponseTypeDef,
+    SlotValueElicitationSettingOutputTypeDef,
+    InitialResponseSettingUnionTypeDef,
+    CreateIntentRequestRequestTypeDef,
+    IntentConfirmationSettingUnionTypeDef,
+    UpdateIntentRequestRequestTypeDef,
     SlotValueElicitationSettingTypeDef,
-    CreateSlotRequestRequestTypeDef,
     CreateSlotResponseTypeDef,
     DescribeSlotResponseTypeDef,
-    UpdateSlotRequestRequestTypeDef,
     UpdateSlotResponseTypeDef,
+    CreateSlotRequestRequestTypeDef,
+    SlotValueElicitationSettingUnionTypeDef,
+    UpdateSlotRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTypeDef:
+def get_value() -> ActiveContextTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/setup.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lexv2-models",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_lexv2_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexModelsV2 2.5.2 service generated with"
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
-    keywords="aiobotocore lexv2-models type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore lexv2-models type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lexv2_models": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/"
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/__init__.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/__init__.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/__main__.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexModelsV2 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.LexModelsV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2\nOther"
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

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/client.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     BotMemberTypeDef,
     BotSortByTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInSlotTypeSortByTypeDef,
-    CompositeSlotTypeSettingTypeDef,
-    ConversationLogSettingsTypeDef,
+    CompositeSlotTypeSettingUnionTypeDef,
+    ConversationLogSettingsUnionTypeDef,
     CreateBotAliasResponseTypeDef,
     CreateBotLocaleResponseTypeDef,
     CreateBotResponseTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateExportResponseTypeDef,
     CreateIntentResponseTypeDef,
     CreateResourcePolicyResponseTypeDef,
@@ -92,23 +92,23 @@
     DialogCodeHookSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     ExportResourceSpecificationTypeDef,
     ExportSortByTypeDef,
     ExternalSourceSettingTypeDef,
-    FulfillmentCodeHookSettingsTypeDef,
+    FulfillmentCodeHookSettingsUnionTypeDef,
     GetTestExecutionArtifactsUrlResponseTypeDef,
     ImportFilterTypeDef,
-    ImportResourceSpecificationTypeDef,
+    ImportResourceSpecificationUnionTypeDef,
     ImportSortByTypeDef,
-    InitialResponseSettingTypeDef,
+    InitialResponseSettingUnionTypeDef,
     InputContextTypeDef,
-    IntentClosingSettingTypeDef,
-    IntentConfirmationSettingTypeDef,
+    IntentClosingSettingUnionTypeDef,
+    IntentConfirmationSettingUnionTypeDef,
     IntentFilterTypeDef,
     IntentSortByTypeDef,
     KendraConfigurationTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
     ListBotAliasesResponseTypeDef,
     ListBotLocalesResponseTypeDef,
     ListBotRecommendationsResponseTypeDef,
@@ -137,31 +137,31 @@
     SearchAssociatedTranscriptsResponseTypeDef,
     SentimentAnalysisSettingsTypeDef,
     SlotFilterTypeDef,
     SlotPriorityTypeDef,
     SlotSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
-    SlotTypeValueTypeDef,
-    SlotValueElicitationSettingTypeDef,
+    SlotTypeValueUnionTypeDef,
+    SlotValueElicitationSettingUnionTypeDef,
     SlotValueSelectionSettingTypeDef,
     StartBotRecommendationResponseTypeDef,
     StartImportResponseTypeDef,
     StartTestExecutionResponseTypeDef,
     StartTestSetGenerationResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
-    SubSlotSettingTypeDef,
+    SubSlotSettingUnionTypeDef,
     TestExecutionResultFilterByTypeDef,
     TestExecutionSortByTypeDef,
     TestExecutionTargetTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
-    TestSetGenerationDataSourceTypeDef,
+    TestSetGenerationDataSourceUnionTypeDef,
     TestSetSortByTypeDef,
     TestSetStorageLocationTypeDef,
-    TranscriptSourceSettingTypeDef,
+    TranscriptSourceSettingUnionTypeDef,
     UpdateBotAliasResponseTypeDef,
     UpdateBotLocaleResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateExportResponseTypeDef,
     UpdateIntentResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
@@ -325,15 +325,15 @@
         self,
         *,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
@@ -392,21 +392,21 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
-        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_intent)
         """
@@ -439,24 +439,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_resource_policy_statement)
         """
 
     async def create_slot(
         self,
         *,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingUnionTypeDef = ...
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_slot)
         """
@@ -465,19 +465,19 @@
         self,
         *,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
     ) -> CreateSlotTypeResponseTypeDef:
         """
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)
@@ -1150,30 +1150,30 @@
 
     async def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        transcriptSourceSetting: TranscriptSourceSettingTypeDef,
+        transcriptSourceSetting: TranscriptSourceSettingUnionTypeDef,
         encryptionSetting: EncryptionSettingTypeDef = ...
     ) -> StartBotRecommendationResponseTypeDef:
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_bot_recommendation)
         """
 
     async def start_import(
         self,
         *,
         importId: str,
-        resourceSpecification: ImportResourceSpecificationTypeDef,
+        resourceSpecification: ImportResourceSpecificationUnionTypeDef,
         mergeStrategy: MergeStrategyType,
         filePassword: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive that
         you uploaded to an S3 bucket.
 
@@ -1197,15 +1197,15 @@
         """
 
     async def start_test_set_generation(
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
-        generationDataSource: TestSetGenerationDataSourceTypeDef,
+        generationDataSource: TestSetGenerationDataSourceUnionTypeDef,
         roleArn: str,
         description: str = ...,
         testSetTags: Mapping[str, str] = ...
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
@@ -1263,15 +1263,15 @@
         *,
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_alias)
@@ -1328,22 +1328,22 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
         slotPriorities: Sequence[SlotPriorityTypeDef] = ...,
-        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_intent)
         """
@@ -1359,24 +1359,24 @@
         """
 
     async def update_slot(
         self,
         *,
         slotId: str,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingUnionTypeDef = ...
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot)
         """
@@ -1386,19 +1386,19 @@
         *,
         slotTypeId: str,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot_type)
         """
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/client.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     BotMemberTypeDef,
     BotSortByTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInSlotTypeSortByTypeDef,
-    CompositeSlotTypeSettingTypeDef,
-    ConversationLogSettingsTypeDef,
+    CompositeSlotTypeSettingUnionTypeDef,
+    ConversationLogSettingsUnionTypeDef,
     CreateBotAliasResponseTypeDef,
     CreateBotLocaleResponseTypeDef,
     CreateBotResponseTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateExportResponseTypeDef,
     CreateIntentResponseTypeDef,
     CreateResourcePolicyResponseTypeDef,
@@ -92,23 +92,23 @@
     DialogCodeHookSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     ExportResourceSpecificationTypeDef,
     ExportSortByTypeDef,
     ExternalSourceSettingTypeDef,
-    FulfillmentCodeHookSettingsTypeDef,
+    FulfillmentCodeHookSettingsUnionTypeDef,
     GetTestExecutionArtifactsUrlResponseTypeDef,
     ImportFilterTypeDef,
-    ImportResourceSpecificationTypeDef,
+    ImportResourceSpecificationUnionTypeDef,
     ImportSortByTypeDef,
-    InitialResponseSettingTypeDef,
+    InitialResponseSettingUnionTypeDef,
     InputContextTypeDef,
-    IntentClosingSettingTypeDef,
-    IntentConfirmationSettingTypeDef,
+    IntentClosingSettingUnionTypeDef,
+    IntentConfirmationSettingUnionTypeDef,
     IntentFilterTypeDef,
     IntentSortByTypeDef,
     KendraConfigurationTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
     ListBotAliasesResponseTypeDef,
     ListBotLocalesResponseTypeDef,
     ListBotRecommendationsResponseTypeDef,
@@ -137,31 +137,31 @@
     SearchAssociatedTranscriptsResponseTypeDef,
     SentimentAnalysisSettingsTypeDef,
     SlotFilterTypeDef,
     SlotPriorityTypeDef,
     SlotSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
-    SlotTypeValueTypeDef,
-    SlotValueElicitationSettingTypeDef,
+    SlotTypeValueUnionTypeDef,
+    SlotValueElicitationSettingUnionTypeDef,
     SlotValueSelectionSettingTypeDef,
     StartBotRecommendationResponseTypeDef,
     StartImportResponseTypeDef,
     StartTestExecutionResponseTypeDef,
     StartTestSetGenerationResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
-    SubSlotSettingTypeDef,
+    SubSlotSettingUnionTypeDef,
     TestExecutionResultFilterByTypeDef,
     TestExecutionSortByTypeDef,
     TestExecutionTargetTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
-    TestSetGenerationDataSourceTypeDef,
+    TestSetGenerationDataSourceUnionTypeDef,
     TestSetSortByTypeDef,
     TestSetStorageLocationTypeDef,
-    TranscriptSourceSettingTypeDef,
+    TranscriptSourceSettingUnionTypeDef,
     UpdateBotAliasResponseTypeDef,
     UpdateBotLocaleResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateExportResponseTypeDef,
     UpdateIntentResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
@@ -313,15 +313,15 @@
         self,
         *,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
@@ -376,21 +376,21 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
-        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_intent)
         """
@@ -420,24 +420,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_resource_policy_statement)
         """
     async def create_slot(
         self,
         *,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingUnionTypeDef = ...
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_slot)
         """
@@ -445,19 +445,19 @@
         self,
         *,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
     ) -> CreateSlotTypeResponseTypeDef:
         """
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)
@@ -1074,29 +1074,29 @@
         """
     async def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        transcriptSourceSetting: TranscriptSourceSettingTypeDef,
+        transcriptSourceSetting: TranscriptSourceSettingUnionTypeDef,
         encryptionSetting: EncryptionSettingTypeDef = ...
     ) -> StartBotRecommendationResponseTypeDef:
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_bot_recommendation)
         """
     async def start_import(
         self,
         *,
         importId: str,
-        resourceSpecification: ImportResourceSpecificationTypeDef,
+        resourceSpecification: ImportResourceSpecificationUnionTypeDef,
         mergeStrategy: MergeStrategyType,
         filePassword: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive that
         you uploaded to an S3 bucket.
 
@@ -1118,15 +1118,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_test_execution)
         """
     async def start_test_set_generation(
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
-        generationDataSource: TestSetGenerationDataSourceTypeDef,
+        generationDataSource: TestSetGenerationDataSourceUnionTypeDef,
         roleArn: str,
         description: str = ...,
         testSetTags: Mapping[str, str] = ...
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
@@ -1179,15 +1179,15 @@
         *,
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_alias)
@@ -1240,22 +1240,22 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
         slotPriorities: Sequence[SlotPriorityTypeDef] = ...,
-        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_intent)
         """
@@ -1269,24 +1269,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_resource_policy)
         """
     async def update_slot(
         self,
         *,
         slotId: str,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingUnionTypeDef = ...
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot)
         """
@@ -1295,19 +1295,19 @@
         *,
         slotTypeId: str,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot_type)
         """
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/literals.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/literals.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/type_defs.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lexv2_models.type_defs import ActiveContextTypeDef
 
-    data: ActiveContextTypeDef = {...}
+    data: ActiveContextTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
     BotFilterNameType,
@@ -75,15 +75,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveContextTypeDef",
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
@@ -93,14 +92,15 @@
     "AssociatedTranscriptTypeDef",
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
     "CustomVocabularyItemTypeDef",
     "FailedCustomVocabularyItemTypeDef",
+    "ResponseMetadataTypeDef",
     "CustomVocabularyEntryIdTypeDef",
     "BotAliasHistoryEventTypeDef",
     "BotAliasSummaryTypeDef",
     "BotAliasTestExecutionTargetTypeDef",
     "BotExportSpecificationTypeDef",
     "BotFilterTypeDef",
     "DataPrivacyTypeDef",
@@ -116,101 +116,86 @@
     "BotRecommendationSummaryTypeDef",
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
     "BotVersionSummaryTypeDef",
     "BuildBotLocaleRequestRequestTypeDef",
-    "BuildBotLocaleResponseTypeDef",
     "BuiltInIntentSortByTypeDef",
     "BuiltInIntentSummaryTypeDef",
     "BuiltInSlotTypeSortByTypeDef",
     "BuiltInSlotTypeSummaryTypeDef",
     "ButtonTypeDef",
     "CloudWatchLogGroupLogDestinationTypeDef",
     "LambdaCodeHookTypeDef",
     "SubSlotTypeCompositionTypeDef",
     "ConditionTypeDef",
     "ConversationLevelIntentClassificationResultItemTypeDef",
     "ConversationLevelResultDetailTypeDef",
     "ConversationLevelSlotResolutionResultItemTypeDef",
     "ConversationLevelTestResultsFilterByTypeDef",
-    "ConversationLogsDataSourceFilterByTypeDef",
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
+    "TimestampTypeDef",
     "SentimentAnalysisSettingsTypeDef",
     "DialogCodeHookSettingsTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "SampleUtteranceTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
-    "CreateResourcePolicyResponseTypeDef",
     "PrincipalTypeDef",
-    "CreateResourcePolicyStatementResponseTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "CustomPayloadTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
-    "DateRangeFilterTypeDef",
+    "DateRangeFilterOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
-    "DeleteBotAliasResponseTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
-    "DeleteBotLocaleResponseTypeDef",
     "DeleteBotRequestRequestTypeDef",
-    "DeleteBotResponseTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
-    "DeleteBotVersionResponseTypeDef",
     "DeleteCustomVocabularyRequestRequestTypeDef",
-    "DeleteCustomVocabularyResponseTypeDef",
     "DeleteExportRequestRequestTypeDef",
-    "DeleteExportResponseTypeDef",
     "DeleteImportRequestRequestTypeDef",
-    "DeleteImportResponseTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
     "DeleteResourcePolicyStatementRequestRequestTypeDef",
-    "DeleteResourcePolicyStatementResponseTypeDef",
     "DeleteSlotRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteTestSetRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
     "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
     "EncryptionSettingTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeExportRequestRequestTypeDef",
     "DescribeImportRequestRequestTypeDef",
     "DescribeIntentRequestRequestTypeDef",
     "SlotPriorityTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSlotRequestRequestTypeDef",
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
     "TestSetStorageLocationTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
     "DialogActionTypeDef",
+    "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportFilterTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
     "IntentFilterTypeDef",
@@ -222,60 +207,78 @@
     "RecommendedIntentSummaryTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
     "PlainTextMessageTypeDef",
     "SSMLMessageTypeDef",
     "OverallTestResultItemTypeDef",
+    "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
     "TextInputSpecificationTypeDef",
     "RelativeAggregationDurationTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
     "SampleValueTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
     "SlotValueTypeDef",
     "SlotValueRegexFilterTypeDef",
     "StopBotRecommendationRequestRequestTypeDef",
-    "StopBotRecommendationResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSetIntentDiscrepancyItemTypeDef",
     "TestSetSlotDiscrepancyItemTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
     "TestSetImportInputLocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
-    "UpdateResourcePolicyResponseTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
-    "SearchAssociatedTranscriptsResponseTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
     "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
-    "ListCustomVocabularyItemsResponseTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
+    "BuildBotLocaleResponseTypeDef",
+    "CreateResourcePolicyResponseTypeDef",
+    "CreateResourcePolicyStatementResponseTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "DeleteBotAliasResponseTypeDef",
+    "DeleteBotLocaleResponseTypeDef",
+    "DeleteBotResponseTypeDef",
+    "DeleteBotVersionResponseTypeDef",
+    "DeleteCustomVocabularyResponseTypeDef",
+    "DeleteExportResponseTypeDef",
+    "DeleteImportResponseTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    "ListCustomVocabularyItemsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    "StopBotRecommendationResponseTypeDef",
+    "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "TestExecutionTargetTypeDef",
+    "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
     "BotLocaleImportSpecificationTypeDef",
     "CreateBotLocaleRequestRequestTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
     "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
@@ -294,37 +297,42 @@
     "CreateBotVersionResponseTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
     "ListBotVersionsResponseTypeDef",
     "ListBuiltInIntentsRequestRequestTypeDef",
     "ListBuiltInIntentsResponseTypeDef",
     "ListBuiltInSlotTypesRequestRequestTypeDef",
     "ListBuiltInSlotTypesResponseTypeDef",
+    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "TextLogDestinationTypeDef",
     "CodeHookSpecificationTypeDef",
+    "CompositeSlotTypeSettingOutputTypeDef",
     "CompositeSlotTypeSettingTypeDef",
     "ConversationLevelTestResultItemTypeDef",
     "TestExecutionResultFilterByTypeDef",
-    "ConversationLogsDataSourceTypeDef",
+    "ConversationLogsDataSourceOutputTypeDef",
+    "ConversationLogsDataSourceFilterByTypeDef",
+    "DateRangeFilterTypeDef",
     "IntentSummaryTypeDef",
     "CreateResourcePolicyStatementRequestRequestTypeDef",
-    "LexTranscriptFilterTypeDef",
+    "LexTranscriptFilterOutputTypeDef",
     "DescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
     "DescribeBotVersionResponseTypeDef",
     "UpdateBotRecommendationRequestRequestTypeDef",
     "DescribeTestSetResponseTypeDef",
     "TestSetSummaryTypeDef",
     "UpdateTestSetResponseTypeDef",
+    "DialogStateOutputTypeDef",
     "DialogStateTypeDef",
     "ExportResourceSpecificationTypeDef",
     "ListExportsRequestRequestTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "InputSessionStateSpecificationTypeDef",
@@ -335,126 +343,174 @@
     "ListSlotTypesResponseTypeDef",
     "ListSlotsRequestRequestTypeDef",
     "ListTestExecutionsRequestRequestTypeDef",
     "ListTestSetsRequestRequestTypeDef",
     "OverallTestResultsTypeDef",
     "UtteranceAggregationDurationTypeDef",
     "RuntimeHintDetailsTypeDef",
+    "SlotTypeValueOutputTypeDef",
     "SlotTypeValueTypeDef",
+    "SlotDefaultValueSpecificationOutputTypeDef",
     "SlotDefaultValueSpecificationTypeDef",
     "SlotResolutionTestResultItemTypeDef",
+    "SlotValueOverrideOutputTypeDef",
     "SlotValueOverrideTypeDef",
     "SlotValueSelectionSettingTypeDef",
     "TestSetDiscrepancyErrorsTypeDef",
     "TestSetDiscrepancyReportResourceTargetTypeDef",
+    "TestSetImportResourceSpecificationOutputTypeDef",
     "TestSetImportResourceSpecificationTypeDef",
     "UserTurnOutputSpecificationTypeDef",
     "UtteranceInputSpecificationTypeDef",
     "PromptAttemptSpecificationTypeDef",
     "AudioLogSettingTypeDef",
     "DescribeTestExecutionResponseTypeDef",
     "StartTestExecutionRequestRequestTypeDef",
     "StartTestExecutionResponseTypeDef",
     "TestExecutionSummaryTypeDef",
     "BotRecommendationResultsTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
     "TextLogSettingTypeDef",
     "BotAliasLocaleSettingsTypeDef",
+    "CompositeSlotTypeSettingUnionTypeDef",
     "ConversationLevelTestResultsTypeDef",
     "ListTestExecutionResultItemsRequestRequestTypeDef",
-    "TestSetGenerationDataSourceTypeDef",
+    "TestSetGenerationDataSourceOutputTypeDef",
+    "ConversationLogsDataSourceTypeDef",
+    "LexTranscriptFilterTypeDef",
     "ListIntentsResponseTypeDef",
-    "TranscriptFilterTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "ListTestSetsResponseTypeDef",
     "CreateExportRequestRequestTypeDef",
     "CreateExportResponseTypeDef",
     "DescribeExportResponseTypeDef",
     "ExportSummaryTypeDef",
     "UpdateExportResponseTypeDef",
     "ExternalSourceSettingTypeDef",
     "IntentClassificationTestResultsTypeDef",
     "ListAggregatedUtterancesRequestRequestTypeDef",
     "ListAggregatedUtterancesResponseTypeDef",
+    "SlotTypeValueUnionTypeDef",
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
+    "ImportResourceSpecificationOutputTypeDef",
     "ImportResourceSpecificationTypeDef",
     "UserTurnInputSpecificationTypeDef",
     "ListTestExecutionsResponseTypeDef",
+    "MessageGroupOutputTypeDef",
     "MessageGroupTypeDef",
+    "ConversationLogSettingsOutputTypeDef",
     "ConversationLogSettingsTypeDef",
     "DescribeTestSetGenerationResponseTypeDef",
-    "StartTestSetGenerationRequestRequestTypeDef",
     "StartTestSetGenerationResponseTypeDef",
-    "S3BucketTranscriptSourceTypeDef",
+    "TestSetGenerationDataSourceTypeDef",
+    "TranscriptFilterTypeDef",
+    "S3BucketTranscriptSourceOutputTypeDef",
     "ListExportsResponseTypeDef",
-    "CreateSlotTypeRequestRequestTypeDef",
     "CreateSlotTypeResponseTypeDef",
     "DescribeSlotTypeResponseTypeDef",
-    "UpdateSlotTypeRequestRequestTypeDef",
     "UpdateSlotTypeResponseTypeDef",
+    "CreateSlotTypeRequestRequestTypeDef",
+    "UpdateSlotTypeRequestRequestTypeDef",
     "IntentLevelSlotResolutionTestResultsTypeDef",
     "DescribeImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
+    "ImportResourceSpecificationUnionTypeDef",
+    "StartImportRequestRequestTypeDef",
     "UserTurnResultTypeDef",
     "UserTurnSpecificationTypeDef",
+    "FulfillmentStartResponseSpecificationOutputTypeDef",
+    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
+    "PromptSpecificationOutputTypeDef",
+    "ResponseSpecificationOutputTypeDef",
+    "StillWaitingResponseSpecificationOutputTypeDef",
     "FulfillmentStartResponseSpecificationTypeDef",
     "FulfillmentUpdateResponseSpecificationTypeDef",
     "PromptSpecificationTypeDef",
     "ResponseSpecificationTypeDef",
     "StillWaitingResponseSpecificationTypeDef",
-    "CreateBotAliasRequestRequestTypeDef",
     "CreateBotAliasResponseTypeDef",
     "DescribeBotAliasResponseTypeDef",
-    "UpdateBotAliasRequestRequestTypeDef",
     "UpdateBotAliasResponseTypeDef",
-    "TranscriptSourceSettingTypeDef",
+    "ConversationLogSettingsUnionTypeDef",
+    "CreateBotAliasRequestRequestTypeDef",
+    "UpdateBotAliasRequestRequestTypeDef",
+    "StartTestSetGenerationRequestRequestTypeDef",
+    "TestSetGenerationDataSourceUnionTypeDef",
+    "S3BucketTranscriptSourceTypeDef",
+    "TranscriptSourceSettingOutputTypeDef",
     "TestSetTurnResultTypeDef",
     "TurnSpecificationTypeDef",
-    "FulfillmentUpdatesSpecificationTypeDef",
+    "FulfillmentUpdatesSpecificationOutputTypeDef",
     "SlotSummaryTypeDef",
+    "ConditionalBranchOutputTypeDef",
+    "DefaultConditionalBranchOutputTypeDef",
+    "WaitAndContinueSpecificationOutputTypeDef",
+    "FulfillmentUpdatesSpecificationTypeDef",
     "ConditionalBranchTypeDef",
     "DefaultConditionalBranchTypeDef",
     "WaitAndContinueSpecificationTypeDef",
+    "TranscriptSourceSettingTypeDef",
     "DescribeBotRecommendationResponseTypeDef",
-    "StartBotRecommendationRequestRequestTypeDef",
     "StartBotRecommendationResponseTypeDef",
     "UpdateBotRecommendationResponseTypeDef",
     "UtteranceLevelTestResultItemTypeDef",
     "TestSetTurnRecordTypeDef",
     "ListSlotsResponseTypeDef",
+    "ConditionalSpecificationOutputTypeDef",
+    "SubSlotValueElicitationSettingOutputTypeDef",
     "ConditionalSpecificationTypeDef",
     "SubSlotValueElicitationSettingTypeDef",
+    "StartBotRecommendationRequestRequestTypeDef",
+    "TranscriptSourceSettingUnionTypeDef",
     "UtteranceLevelTestResultsTypeDef",
     "ListTestSetRecordsResponseTypeDef",
+    "IntentClosingSettingOutputTypeDef",
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    "SpecificationsOutputTypeDef",
     "IntentClosingSettingTypeDef",
     "PostDialogCodeHookInvocationSpecificationTypeDef",
     "PostFulfillmentStatusSpecificationTypeDef",
     "SpecificationsTypeDef",
     "TestExecutionResultItemsTypeDef",
+    "DialogCodeHookInvocationSettingOutputTypeDef",
+    "FulfillmentCodeHookSettingsOutputTypeDef",
+    "SubSlotSettingOutputTypeDef",
+    "IntentClosingSettingUnionTypeDef",
     "DialogCodeHookInvocationSettingTypeDef",
     "FulfillmentCodeHookSettingsTypeDef",
     "SubSlotSettingTypeDef",
     "ListTestExecutionResultItemsResponseTypeDef",
+    "InitialResponseSettingOutputTypeDef",
+    "IntentConfirmationSettingOutputTypeDef",
+    "SlotCaptureSettingOutputTypeDef",
     "InitialResponseSettingTypeDef",
     "IntentConfirmationSettingTypeDef",
     "SlotCaptureSettingTypeDef",
-    "CreateIntentRequestRequestTypeDef",
+    "FulfillmentCodeHookSettingsUnionTypeDef",
+    "SubSlotSettingUnionTypeDef",
     "CreateIntentResponseTypeDef",
     "DescribeIntentResponseTypeDef",
-    "UpdateIntentRequestRequestTypeDef",
     "UpdateIntentResponseTypeDef",
+    "SlotValueElicitationSettingOutputTypeDef",
+    "InitialResponseSettingUnionTypeDef",
+    "CreateIntentRequestRequestTypeDef",
+    "IntentConfirmationSettingUnionTypeDef",
+    "UpdateIntentRequestRequestTypeDef",
     "SlotValueElicitationSettingTypeDef",
-    "CreateSlotRequestRequestTypeDef",
     "CreateSlotResponseTypeDef",
     "DescribeSlotResponseTypeDef",
-    "UpdateSlotRequestRequestTypeDef",
     "UpdateSlotResponseTypeDef",
+    "CreateSlotRequestRequestTypeDef",
+    "SlotValueElicitationSettingUnionTypeDef",
+    "UpdateSlotRequestRequestTypeDef",
 )
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
     },
@@ -566,21 +622,19 @@
     "_OptionalS3BucketLogDestinationTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class S3BucketLogDestinationTypeDef(
     _RequiredS3BucketLogDestinationTypeDef, _OptionalS3BucketLogDestinationTypeDef
 ):
     pass
 
-
 _RequiredNewCustomVocabularyItemTypeDef = TypedDict(
     "_RequiredNewCustomVocabularyItemTypeDef",
     {
         "phrase": str,
     },
 )
 _OptionalNewCustomVocabularyItemTypeDef = TypedDict(
@@ -588,21 +642,19 @@
     {
         "weight": int,
         "displayAs": str,
     },
     total=False,
 )
 
-
 class NewCustomVocabularyItemTypeDef(
     _RequiredNewCustomVocabularyItemTypeDef, _OptionalNewCustomVocabularyItemTypeDef
 ):
     pass
 
-
 _RequiredCustomVocabularyItemTypeDef = TypedDict(
     "_RequiredCustomVocabularyItemTypeDef",
     {
         "itemId": str,
         "phrase": str,
     },
 )
@@ -611,31 +663,40 @@
     {
         "weight": int,
         "displayAs": str,
     },
     total=False,
 )
 
-
 class CustomVocabularyItemTypeDef(
     _RequiredCustomVocabularyItemTypeDef, _OptionalCustomVocabularyItemTypeDef
 ):
     pass
 
-
 FailedCustomVocabularyItemTypeDef = TypedDict(
     "FailedCustomVocabularyItemTypeDef",
     {
         "itemId": str,
         "errorMessage": str,
         "errorCode": ErrorCodeType,
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
 CustomVocabularyEntryIdTypeDef = TypedDict(
     "CustomVocabularyEntryIdTypeDef",
     {
         "itemId": str,
     },
 )
 
@@ -732,19 +793,17 @@
     "_OptionalVoiceSettingsTypeDef",
     {
         "engine": VoiceEngineType,
     },
     total=False,
 )
 
-
 class VoiceSettingsTypeDef(_RequiredVoiceSettingsTypeDef, _OptionalVoiceSettingsTypeDef):
     pass
 
-
 BotLocaleSortByTypeDef = TypedDict(
     "BotLocaleSortByTypeDef",
     {
         "attribute": Literal["BotLocaleName"],
         "order": SortOrderType,
     },
 )
@@ -801,21 +860,19 @@
     {
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-
 class BotRecommendationSummaryTypeDef(
     _RequiredBotRecommendationSummaryTypeDef, _OptionalBotRecommendationSummaryTypeDef
 ):
     pass
 
-
 BotSortByTypeDef = TypedDict(
     "BotSortByTypeDef",
     {
         "attribute": Literal["BotName"],
         "order": SortOrderType,
     },
 )
@@ -866,26 +923,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-BuildBotLocaleResponseTypeDef = TypedDict(
-    "BuildBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "lastBuildSubmittedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BuiltInIntentSortByTypeDef = TypedDict(
     "BuiltInIntentSortByTypeDef",
     {
         "attribute": Literal["IntentSignature"],
         "order": SortOrderType,
     },
 )
@@ -973,21 +1018,19 @@
     "_OptionalConversationLevelResultDetailTypeDef",
     {
         "speechTranscriptionResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-
 class ConversationLevelResultDetailTypeDef(
     _RequiredConversationLevelResultDetailTypeDef, _OptionalConversationLevelResultDetailTypeDef
 ):
     pass
 
-
 ConversationLevelSlotResolutionResultItemTypeDef = TypedDict(
     "ConversationLevelSlotResolutionResultItemTypeDef",
     {
         "intentName": str,
         "slotName": str,
         "matchResult": TestResultMatchStatusType,
     },
@@ -997,23 +1040,24 @@
     "ConversationLevelTestResultsFilterByTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-ConversationLogsDataSourceFilterByTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByTypeDef",
+ConversationLogsDataSourceFilterByOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
         "inputMode": ConversationLogsInputModeFilterType,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 SentimentAnalysisSettingsTypeDef = TypedDict(
     "SentimentAnalysisSettingsTypeDef",
     {
         "detectSentiment": bool,
     },
 )
 
@@ -1042,21 +1086,19 @@
     {
         "queryFilterStringEnabled": bool,
         "queryFilterString": str,
     },
     total=False,
 )
 
-
 class KendraConfigurationTypeDef(
     _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
 ):
     pass
 
-
 OutputContextTypeDef = TypedDict(
     "OutputContextTypeDef",
     {
         "name": str,
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
@@ -1073,41 +1115,23 @@
     "CreateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
 
-CreateResourcePolicyResponseTypeDef = TypedDict(
-    "CreateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "service": str,
         "arn": str,
     },
     total=False,
 )
 
-CreateResourcePolicyStatementResponseTypeDef = TypedDict(
-    "CreateResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MultipleValuesSettingTypeDef = TypedDict(
     "MultipleValuesSettingTypeDef",
     {
         "allowMultipleValues": bool,
     },
     total=False,
 )
@@ -1115,23 +1139,14 @@
 ObfuscationSettingTypeDef = TypedDict(
     "ObfuscationSettingTypeDef",
     {
         "obfuscationSettingType": ObfuscationSettingTypeType,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "importId": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomPayloadTypeDef = TypedDict(
     "CustomPayloadTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1149,16 +1164,16 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DateRangeFilterTypeDef = TypedDict(
-    "DateRangeFilterTypeDef",
+DateRangeFilterOutputTypeDef = TypedDict(
+    "DateRangeFilterOutputTypeDef",
     {
         "startDateTime": datetime,
         "endDateTime": datetime,
     },
 )
 
 _RequiredDeleteBotAliasRequestRequestTypeDef = TypedDict(
@@ -1172,81 +1187,47 @@
     "_OptionalDeleteBotAliasRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
-
 class DeleteBotAliasRequestRequestTypeDef(
     _RequiredDeleteBotAliasRequestRequestTypeDef, _OptionalDeleteBotAliasRequestRequestTypeDef
 ):
     pass
 
-
-DeleteBotAliasResponseTypeDef = TypedDict(
-    "DeleteBotAliasResponseTypeDef",
-    {
-        "botAliasId": str,
-        "botId": str,
-        "botAliasStatus": BotAliasStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBotLocaleRequestRequestTypeDef = TypedDict(
     "DeleteBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteBotLocaleResponseTypeDef = TypedDict(
-    "DeleteBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalDeleteBotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBotRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
-
 class DeleteBotRequestRequestTypeDef(
     _RequiredDeleteBotRequestRequestTypeDef, _OptionalDeleteBotRequestRequestTypeDef
 ):
     pass
 
-
-DeleteBotResponseTypeDef = TypedDict(
-    "DeleteBotResponseTypeDef",
-    {
-        "botId": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotVersionRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -1254,83 +1235,42 @@
     "_OptionalDeleteBotVersionRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
-
 class DeleteBotVersionRequestRequestTypeDef(
     _RequiredDeleteBotVersionRequestRequestTypeDef, _OptionalDeleteBotVersionRequestRequestTypeDef
 ):
     pass
 
-
-DeleteBotVersionResponseTypeDef = TypedDict(
-    "DeleteBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCustomVocabularyRequestRequestTypeDef = TypedDict(
     "DeleteCustomVocabularyRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteCustomVocabularyResponseTypeDef = TypedDict(
-    "DeleteCustomVocabularyResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteExportRequestRequestTypeDef = TypedDict(
     "DeleteExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-DeleteExportResponseTypeDef = TypedDict(
-    "DeleteExportResponseTypeDef",
-    {
-        "exportId": str,
-        "exportStatus": ExportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImportRequestRequestTypeDef = TypedDict(
     "DeleteImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-DeleteImportResponseTypeDef = TypedDict(
-    "DeleteImportResponseTypeDef",
-    {
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIntentRequestRequestTypeDef = TypedDict(
     "DeleteIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -1347,31 +1287,20 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "expectedRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourcePolicyStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "statementId": str,
     },
 )
@@ -1379,31 +1308,20 @@
     "_OptionalDeleteResourcePolicyStatementRequestRequestTypeDef",
     {
         "expectedRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteResourcePolicyStatementRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSlotRequestRequestTypeDef = TypedDict(
     "DeleteSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -1424,21 +1342,19 @@
     "_OptionalDeleteSlotTypeRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
-
 class DeleteSlotTypeRequestRequestTypeDef(
     _RequiredDeleteSlotTypeRequestRequestTypeDef, _OptionalDeleteSlotTypeRequestRequestTypeDef
 ):
     pass
 
-
 DeleteTestSetRequestRequestTypeDef = TypedDict(
     "DeleteTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
     },
 )
 
@@ -1453,21 +1369,19 @@
     {
         "localeId": str,
         "sessionId": str,
     },
     total=False,
 )
 
-
 class DeleteUtterancesRequestRequestTypeDef(
     _RequiredDeleteUtterancesRequestRequestTypeDef, _OptionalDeleteUtterancesRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1538,27 +1452,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExportRequestRequestTypeDef = TypedDict(
     "DescribeExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
@@ -1590,24 +1491,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSlotRequestRequestTypeDef = TypedDict(
     "DescribeSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -1657,21 +1548,19 @@
     "_OptionalTestSetStorageLocationTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class TestSetStorageLocationTypeDef(
     _RequiredTestSetStorageLocationTypeDef, _OptionalTestSetStorageLocationTypeDef
 ):
     pass
 
-
 DescribeTestSetRequestRequestTypeDef = TypedDict(
     "DescribeTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
     },
 )
 
@@ -1686,18 +1575,25 @@
     {
         "slotToElicit": str,
         "suppressNextMessage": bool,
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+IntentOverrideOutputTypeDef = TypedDict(
+    "IntentOverrideOutputTypeDef",
+    {
+        "name": str,
+        "slots": Dict[str, "SlotValueOverrideOutputTypeDef"],
+    },
+    total=False,
+)
 
 IntentOverrideTypeDef = TypedDict(
     "IntentOverrideTypeDef",
     {
         "name": str,
         "slots": Mapping[str, "SlotValueOverrideTypeDef"],
     },
@@ -1714,29 +1610,20 @@
     "_OptionalElicitationCodeHookInvocationSettingTypeDef",
     {
         "invocationLabel": str,
     },
     total=False,
 )
 
-
 class ElicitationCodeHookInvocationSettingTypeDef(
     _RequiredElicitationCodeHookInvocationSettingTypeDef,
     _OptionalElicitationCodeHookInvocationSettingTypeDef,
 ):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportFilterTypeDef = TypedDict(
     "ExportFilterTypeDef",
     {
         "name": Literal["ExportResourceType"],
         "values": Sequence[str],
         "operator": ExportFilterOperatorType,
     },
@@ -1760,23 +1647,14 @@
 GetTestExecutionArtifactsUrlRequestRequestTypeDef = TypedDict(
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     {
         "testExecutionId": str,
     },
 )
 
-GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
-    {
-        "testExecutionId": str,
-        "downloadArtifactsUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGrammarSlotTypeSourceTypeDef = TypedDict(
     "_RequiredGrammarSlotTypeSourceTypeDef",
     {
         "s3BucketName": str,
         "s3ObjectKey": str,
     },
 )
@@ -1784,21 +1662,19 @@
     "_OptionalGrammarSlotTypeSourceTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class GrammarSlotTypeSourceTypeDef(
     _RequiredGrammarSlotTypeSourceTypeDef, _OptionalGrammarSlotTypeSourceTypeDef
 ):
     pass
 
-
 ImportFilterTypeDef = TypedDict(
     "ImportFilterTypeDef",
     {
         "name": Literal["ImportResourceType"],
         "values": Sequence[str],
         "operator": ImportFilterOperatorType,
     },
@@ -1846,22 +1722,20 @@
     "_OptionalIntentClassificationTestResultItemCountsTypeDef",
     {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
     },
     total=False,
 )
 
-
 class IntentClassificationTestResultItemCountsTypeDef(
     _RequiredIntentClassificationTestResultItemCountsTypeDef,
     _OptionalIntentClassificationTestResultItemCountsTypeDef,
 ):
     pass
 
-
 IntentFilterTypeDef = TypedDict(
     "IntentFilterTypeDef",
     {
         "name": Literal["IntentName"],
         "values": Sequence[str],
         "operator": IntentFilterOperatorType,
     },
@@ -1886,21 +1760,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBotAliasesRequestRequestTypeDef(
     _RequiredListBotAliasesRequestRequestTypeDef, _OptionalListBotAliasesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListBotRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotRecommendationsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -1910,22 +1782,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBotRecommendationsRequestRequestTypeDef(
     _RequiredListBotRecommendationsRequestRequestTypeDef,
     _OptionalListBotRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListCustomVocabularyItemsRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomVocabularyItemsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -1935,22 +1805,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListCustomVocabularyItemsRequestRequestTypeDef(
     _RequiredListCustomVocabularyItemsRequestRequestTypeDef,
     _OptionalListCustomVocabularyItemsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListRecommendedIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendedIntentsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -1961,22 +1829,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListRecommendedIntentsRequestRequestTypeDef(
     _RequiredListRecommendedIntentsRequestRequestTypeDef,
     _OptionalListRecommendedIntentsRequestRequestTypeDef,
 ):
     pass
 
-
 RecommendedIntentSummaryTypeDef = TypedDict(
     "RecommendedIntentSummaryTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "sampleUtterancesCount": int,
     },
@@ -2033,22 +1899,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
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
 TestExecutionSortByTypeDef = TypedDict(
     "TestExecutionSortByTypeDef",
     {
         "attribute": TestExecutionSortAttributeType,
         "order": SortOrderType,
     },
 )
@@ -2064,22 +1922,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTestSetRecordsRequestRequestTypeDef(
     _RequiredListTestSetRecordsRequestRequestTypeDef,
     _OptionalListTestSetRecordsRequestRequestTypeDef,
 ):
     pass
 
-
 TestSetSortByTypeDef = TypedDict(
     "TestSetSortByTypeDef",
     {
         "attribute": TestSetSortAttributeType,
         "order": SortOrderType,
     },
 )
@@ -2110,25 +1966,31 @@
     "_OptionalOverallTestResultItemTypeDef",
     {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
     },
     total=False,
 )
 
-
 class OverallTestResultItemTypeDef(
     _RequiredOverallTestResultItemTypeDef, _OptionalOverallTestResultItemTypeDef
 ):
     pass
 
+PathFormatOutputTypeDef = TypedDict(
+    "PathFormatOutputTypeDef",
+    {
+        "objectPrefixes": List[str],
+    },
+    total=False,
+)
 
 PathFormatTypeDef = TypedDict(
     "PathFormatTypeDef",
     {
-        "objectPrefixes": List[str],
+        "objectPrefixes": Sequence[str],
     },
     total=False,
 )
 
 TextInputSpecificationTypeDef = TypedDict(
     "TextInputSpecificationTypeDef",
     {
@@ -2140,25 +2002,14 @@
     "RelativeAggregationDurationTypeDef",
     {
         "timeDimension": TimeDimensionType,
         "timeValue": int,
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
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -2187,22 +2038,20 @@
     "_OptionalSlotResolutionTestResultItemCountsTypeDef",
     {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
     },
     total=False,
 )
 
-
 class SlotResolutionTestResultItemCountsTypeDef(
     _RequiredSlotResolutionTestResultItemCountsTypeDef,
     _OptionalSlotResolutionTestResultItemCountsTypeDef,
 ):
     pass
 
-
 SlotValueTypeDef = TypedDict(
     "SlotValueTypeDef",
     {
         "interpretedValue": str,
     },
     total=False,
 )
@@ -2220,26 +2069,14 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
     },
 )
 
-StopBotRecommendationResponseTypeDef = TypedDict(
-    "StopBotRecommendationResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationStatus": BotRecommendationStatusType,
-        "botRecommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2296,21 +2133,19 @@
     "_OptionalUpdateExportRequestRequestTypeDef",
     {
         "filePassword": str,
     },
     total=False,
 )
 
-
 class UpdateExportRequestRequestTypeDef(
     _RequiredUpdateExportRequestRequestTypeDef, _OptionalUpdateExportRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
@@ -2318,31 +2153,20 @@
     "_OptionalUpdateResourcePolicyRequestRequestTypeDef",
     {
         "expectedRevisionId": str,
     },
     total=False,
 )
 
-
 class UpdateResourcePolicyRequestRequestTypeDef(
     _RequiredUpdateResourcePolicyRequestRequestTypeDef,
     _OptionalUpdateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateResourcePolicyResponseTypeDef = TypedDict(
-    "UpdateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTestSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
     },
 )
@@ -2350,42 +2174,38 @@
     "_OptionalUpdateTestSetRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateTestSetRequestRequestTypeDef(
     _RequiredUpdateTestSetRequestRequestTypeDef, _OptionalUpdateTestSetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUserTurnIntentOutputTypeDef = TypedDict(
     "_RequiredUserTurnIntentOutputTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUserTurnIntentOutputTypeDef = TypedDict(
     "_OptionalUserTurnIntentOutputTypeDef",
     {
         "slots": Dict[str, "UserTurnSlotOutputTypeDef"],
     },
     total=False,
 )
 
-
 class UserTurnIntentOutputTypeDef(
     _RequiredUserTurnIntentOutputTypeDef, _OptionalUserTurnIntentOutputTypeDef
 ):
     pass
 
-
 UserTurnSlotOutputTypeDef = TypedDict(
     "UserTurnSlotOutputTypeDef",
     {
         "value": str,
         "values": List[Dict[str, Any]],
         "subSlots": Dict[str, Dict[str, Any]],
     },
@@ -2412,19 +2232,17 @@
         "errorDetails": ExecutionErrorDetailsTypeDef,
         "actualElicitedSlot": str,
         "actualIntent": str,
     },
     total=False,
 )
 
-
 class AgentTurnResultTypeDef(_RequiredAgentTurnResultTypeDef, _OptionalAgentTurnResultTypeDef):
     pass
 
-
 _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAssociatedTranscriptsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -2437,36 +2255,20 @@
         "searchOrder": SearchOrderType,
         "maxResults": int,
         "nextIndex": int,
     },
     total=False,
 )
 
-
 class SearchAssociatedTranscriptsRequestRequestTypeDef(
     _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef,
     _OptionalSearchAssociatedTranscriptsRequestRequestTypeDef,
 ):
     pass
 
-
-SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
-    "SearchAssociatedTranscriptsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationId": str,
-        "nextIndex": int,
-        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
-        "totalResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAudioAndDTMFInputSpecificationTypeDef = TypedDict(
     "_RequiredAudioAndDTMFInputSpecificationTypeDef",
     {
         "startTimeoutMs": int,
     },
 )
 _OptionalAudioAndDTMFInputSpecificationTypeDef = TypedDict(
@@ -2474,21 +2276,19 @@
     {
         "audioSpecification": AudioSpecificationTypeDef,
         "dtmfSpecification": DTMFSpecificationTypeDef,
     },
     total=False,
 )
 
-
 class AudioAndDTMFInputSpecificationTypeDef(
     _RequiredAudioAndDTMFInputSpecificationTypeDef, _OptionalAudioAndDTMFInputSpecificationTypeDef
 ):
     pass
 
-
 AudioLogDestinationTypeDef = TypedDict(
     "AudioLogDestinationTypeDef",
     {
         "s3Bucket": S3BucketLogDestinationTypeDef,
     },
 )
 
@@ -2508,59 +2308,267 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[CustomVocabularyItemTypeDef],
     },
 )
 
-ListCustomVocabularyItemsResponseTypeDef = TypedDict(
-    "ListCustomVocabularyItemsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyItems": List[CustomVocabularyItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchCreateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BuildBotLocaleResponseTypeDef = TypedDict(
+    "BuildBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "lastBuildSubmittedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyResponseTypeDef = TypedDict(
+    "CreateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyStatementResponseTypeDef = TypedDict(
+    "CreateResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "importId": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotAliasResponseTypeDef = TypedDict(
+    "DeleteBotAliasResponseTypeDef",
+    {
+        "botAliasId": str,
+        "botId": str,
+        "botAliasStatus": BotAliasStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotLocaleResponseTypeDef = TypedDict(
+    "DeleteBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotResponseTypeDef = TypedDict(
+    "DeleteBotResponseTypeDef",
+    {
+        "botId": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotVersionResponseTypeDef = TypedDict(
+    "DeleteBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomVocabularyResponseTypeDef = TypedDict(
+    "DeleteCustomVocabularyResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteExportResponseTypeDef = TypedDict(
+    "DeleteExportResponseTypeDef",
+    {
+        "exportId": str,
+        "exportStatus": ExportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImportResponseTypeDef = TypedDict(
+    "DeleteImportResponseTypeDef",
+    {
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "policy": str,
+        "revisionId": str,
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
+GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    {
+        "testExecutionId": str,
+        "downloadArtifactsUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVocabularyItemsResponseTypeDef = TypedDict(
+    "ListCustomVocabularyItemsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyItems": List[CustomVocabularyItemTypeDef],
+        "nextToken": str,
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
+SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationId": str,
+        "nextIndex": int,
+        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
+        "totalResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopBotRecommendationResponseTypeDef = TypedDict(
+    "StopBotRecommendationResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationStatus": BotRecommendationStatusType,
+        "botRecommendationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateResourcePolicyResponseTypeDef = TypedDict(
+    "UpdateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemRequestRequestTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     {
         "botId": str,
@@ -2572,51 +2580,72 @@
 
 ListBotAliasesResponseTypeDef = TypedDict(
     "ListBotAliasesResponseTypeDef",
     {
         "botAliasSummaries": List[BotAliasSummaryTypeDef],
         "nextToken": str,
         "botId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionTargetTypeDef = TypedDict(
     "TestExecutionTargetTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetTypeDef,
     },
     total=False,
 )
 
+_RequiredBotImportSpecificationOutputTypeDef = TypedDict(
+    "_RequiredBotImportSpecificationOutputTypeDef",
+    {
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+    },
+)
+_OptionalBotImportSpecificationOutputTypeDef = TypedDict(
+    "_OptionalBotImportSpecificationOutputTypeDef",
+    {
+        "idleSessionTTLInSeconds": int,
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
+    },
+    total=False,
+)
+
+class BotImportSpecificationOutputTypeDef(
+    _RequiredBotImportSpecificationOutputTypeDef, _OptionalBotImportSpecificationOutputTypeDef
+):
+    pass
+
 _RequiredBotImportSpecificationTypeDef = TypedDict(
     "_RequiredBotImportSpecificationTypeDef",
     {
         "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
     },
 )
 _OptionalBotImportSpecificationTypeDef = TypedDict(
     "_OptionalBotImportSpecificationTypeDef",
     {
         "idleSessionTTLInSeconds": int,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
     pass
 
-
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2626,21 +2655,19 @@
     {
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class BotLocaleImportSpecificationTypeDef(
     _RequiredBotLocaleImportSpecificationTypeDef, _OptionalBotLocaleImportSpecificationTypeDef
 ):
     pass
 
-
 _RequiredCreateBotLocaleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "nluIntentConfidenceThreshold": float,
@@ -2651,34 +2678,32 @@
     {
         "description": str,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateBotLocaleRequestRequestTypeDef(
     _RequiredCreateBotLocaleRequestRequestTypeDef, _OptionalCreateBotLocaleRequestRequestTypeDef
 ):
     pass
 
-
 CreateBotLocaleResponseTypeDef = TypedDict(
     "CreateBotLocaleResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeName": str,
         "localeId": str,
         "description": str,
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotLocaleResponseTypeDef = TypedDict(
     "DescribeBotLocaleResponseTypeDef",
     {
         "botId": str,
@@ -2693,15 +2718,15 @@
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
         "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBotLocaleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
@@ -2715,21 +2740,19 @@
     {
         "description": str,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBotLocaleRequestRequestTypeDef(
     _RequiredUpdateBotLocaleRequestRequestTypeDef, _OptionalUpdateBotLocaleRequestRequestTypeDef
 ):
     pass
 
-
 UpdateBotLocaleResponseTypeDef = TypedDict(
     "UpdateBotLocaleResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "localeName": str,
@@ -2737,15 +2760,15 @@
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBotLocalesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotLocalesRequestRequestTypeDef",
     {
         "botId": str,
@@ -2759,29 +2782,27 @@
         "filters": Sequence[BotLocaleFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBotLocalesRequestRequestTypeDef(
     _RequiredListBotLocalesRequestRequestTypeDef, _OptionalListBotLocalesRequestRequestTypeDef
 ):
     pass
 
-
 ListBotLocalesResponseTypeDef = TypedDict(
     "ListBotLocalesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "botName": str,
@@ -2798,21 +2819,19 @@
         "testBotAliasTags": Mapping[str, str],
         "botType": BotTypeType,
         "botMembers": Sequence[BotMemberTypeDef],
     },
     total=False,
 )
 
-
 class CreateBotRequestRequestTypeDef(
     _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
 ):
     pass
 
-
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
@@ -2820,15 +2839,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "botTags": Dict[str, str],
         "testBotAliasTags": Dict[str, str],
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotResponseTypeDef = TypedDict(
     "DescribeBotResponseTypeDef",
     {
         "botId": str,
@@ -2839,15 +2858,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "botId": str,
@@ -2863,36 +2882,34 @@
         "description": str,
         "botType": BotTypeType,
         "botMembers": Sequence[BotMemberTypeDef],
     },
     total=False,
 )
 
-
 class UpdateBotRequestRequestTypeDef(
     _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
 ):
     pass
 
-
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BotRecommendationResultStatisticsTypeDef = TypedDict(
     "BotRecommendationResultStatisticsTypeDef",
     {
         "intents": IntentStatisticsTypeDef,
@@ -2905,15 +2922,15 @@
     "ListBotRecommendationsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationSummaries": List[BotRecommendationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsRequestRequestTypeDef = TypedDict(
     "ListBotsRequestRequestTypeDef",
     {
         "sortBy": BotSortByTypeDef,
@@ -2925,15 +2942,15 @@
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "botSummaries": List[BotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotVersionRequestRequestTypeDef",
     {
         "botId": str,
@@ -2944,31 +2961,29 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "botId": str,
         "description": str,
         "botVersion": str,
         "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsTypeDef],
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotVersionsRequestRequestTypeDef",
     {
         "botId": str,
@@ -2980,28 +2995,26 @@
         "sortBy": BotVersionSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBotVersionsRequestRequestTypeDef(
     _RequiredListBotVersionsRequestRequestTypeDef, _OptionalListBotVersionsRequestRequestTypeDef
 ):
     pass
 
-
 ListBotVersionsResponseTypeDef = TypedDict(
     "ListBotVersionsResponseTypeDef",
     {
         "botId": str,
         "botVersionSummaries": List[BotVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInIntentsRequestRequestTypeDef",
     {
         "localeId": str,
@@ -3013,29 +3026,27 @@
         "sortBy": BuiltInIntentSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBuiltInIntentsRequestRequestTypeDef(
     _RequiredListBuiltInIntentsRequestRequestTypeDef,
     _OptionalListBuiltInIntentsRequestRequestTypeDef,
 ):
     pass
 
-
 ListBuiltInIntentsResponseTypeDef = TypedDict(
     "ListBuiltInIntentsResponseTypeDef",
     {
         "builtInIntentSummaries": List[BuiltInIntentSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInSlotTypesRequestRequestTypeDef",
     {
         "localeId": str,
@@ -3047,32 +3058,51 @@
         "sortBy": BuiltInSlotTypeSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBuiltInSlotTypesRequestRequestTypeDef(
     _RequiredListBuiltInSlotTypesRequestRequestTypeDef,
     _OptionalListBuiltInSlotTypesRequestRequestTypeDef,
 ):
     pass
 
-
 ListBuiltInSlotTypesResponseTypeDef = TypedDict(
     "ListBuiltInSlotTypesResponseTypeDef",
     {
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImageResponseCardOutputTypeDef = TypedDict(
+    "_RequiredImageResponseCardOutputTypeDef",
+    {
+        "title": str,
+    },
+)
+_OptionalImageResponseCardOutputTypeDef = TypedDict(
+    "_OptionalImageResponseCardOutputTypeDef",
+    {
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+class ImageResponseCardOutputTypeDef(
+    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
+):
+    pass
+
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
@@ -3081,35 +3111,41 @@
         "subtitle": str,
         "imageUrl": str,
         "buttons": Sequence[ButtonTypeDef],
     },
     total=False,
 )
 
-
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
-
 TextLogDestinationTypeDef = TypedDict(
     "TextLogDestinationTypeDef",
     {
         "cloudWatch": CloudWatchLogGroupLogDestinationTypeDef,
     },
 )
 
 CodeHookSpecificationTypeDef = TypedDict(
     "CodeHookSpecificationTypeDef",
     {
         "lambdaCodeHook": LambdaCodeHookTypeDef,
     },
 )
 
+CompositeSlotTypeSettingOutputTypeDef = TypedDict(
+    "CompositeSlotTypeSettingOutputTypeDef",
+    {
+        "subSlots": List[SubSlotTypeCompositionTypeDef],
+    },
+    total=False,
+)
+
 CompositeSlotTypeSettingTypeDef = TypedDict(
     "CompositeSlotTypeSettingTypeDef",
     {
         "subSlots": Sequence[SubSlotTypeCompositionTypeDef],
     },
     total=False,
 )
@@ -3127,49 +3163,62 @@
     "_OptionalConversationLevelTestResultItemTypeDef",
     {
         "speechTranscriptionResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-
 class ConversationLevelTestResultItemTypeDef(
     _RequiredConversationLevelTestResultItemTypeDef, _OptionalConversationLevelTestResultItemTypeDef
 ):
     pass
 
-
 _RequiredTestExecutionResultFilterByTypeDef = TypedDict(
     "_RequiredTestExecutionResultFilterByTypeDef",
     {
         "resultTypeFilter": TestResultTypeFilterType,
     },
 )
 _OptionalTestExecutionResultFilterByTypeDef = TypedDict(
     "_OptionalTestExecutionResultFilterByTypeDef",
     {
         "conversationLevelTestResultsFilterBy": ConversationLevelTestResultsFilterByTypeDef,
     },
     total=False,
 )
 
-
 class TestExecutionResultFilterByTypeDef(
     _RequiredTestExecutionResultFilterByTypeDef, _OptionalTestExecutionResultFilterByTypeDef
 ):
     pass
 
-
-ConversationLogsDataSourceTypeDef = TypedDict(
-    "ConversationLogsDataSourceTypeDef",
+ConversationLogsDataSourceOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceOutputTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
-        "filter": ConversationLogsDataSourceFilterByTypeDef,
+        "filter": ConversationLogsDataSourceFilterByOutputTypeDef,
+    },
+)
+
+ConversationLogsDataSourceFilterByTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "inputMode": ConversationLogsInputModeFilterType,
+    },
+)
+
+DateRangeFilterTypeDef = TypedDict(
+    "DateRangeFilterTypeDef",
+    {
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
     },
 )
 
 IntentSummaryTypeDef = TypedDict(
     "IntentSummaryTypeDef",
     {
         "intentId": str,
@@ -3198,26 +3247,24 @@
     {
         "condition": Mapping[str, Mapping[str, str]],
         "expectedRevisionId": str,
     },
     total=False,
 )
 
-
 class CreateResourcePolicyStatementRequestRequestTypeDef(
     _RequiredCreateResourcePolicyStatementRequestRequestTypeDef,
     _OptionalCreateResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
-
-LexTranscriptFilterTypeDef = TypedDict(
-    "LexTranscriptFilterTypeDef",
+LexTranscriptFilterOutputTypeDef = TypedDict(
+    "LexTranscriptFilterOutputTypeDef",
     {
-        "dateRangeFilter": DateRangeFilterTypeDef,
+        "dateRangeFilter": DateRangeFilterOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     {
@@ -3229,22 +3276,20 @@
     "_OptionalDescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBotAliasRequestBotAliasAvailableWaitTypeDef(
     _RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     _OptionalDescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef = TypedDict(
     "_RequiredDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3253,22 +3298,20 @@
     "_OptionalDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef(
     _RequiredDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     _OptionalDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3277,22 +3320,20 @@
     "_OptionalDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef(
     _RequiredDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     _OptionalDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3301,44 +3342,40 @@
     "_OptionalDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef(
     _RequiredDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     _OptionalDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBotRequestBotAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotRequestBotAvailableWaitTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalDescribeBotRequestBotAvailableWaitTypeDef = TypedDict(
     "_OptionalDescribeBotRequestBotAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBotRequestBotAvailableWaitTypeDef(
     _RequiredDescribeBotRequestBotAvailableWaitTypeDef,
     _OptionalDescribeBotRequestBotAvailableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBotVersionRequestBotVersionAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -3346,66 +3383,60 @@
     "_OptionalDescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBotVersionRequestBotVersionAvailableWaitTypeDef(
     _RequiredDescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     _OptionalDescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeExportRequestBotExportCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeExportRequestBotExportCompletedWaitTypeDef",
     {
         "exportId": str,
     },
 )
 _OptionalDescribeExportRequestBotExportCompletedWaitTypeDef = TypedDict(
     "_OptionalDescribeExportRequestBotExportCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeExportRequestBotExportCompletedWaitTypeDef(
     _RequiredDescribeExportRequestBotExportCompletedWaitTypeDef,
     _OptionalDescribeExportRequestBotExportCompletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImportRequestBotImportCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeImportRequestBotImportCompletedWaitTypeDef",
     {
         "importId": str,
     },
 )
 _OptionalDescribeImportRequestBotImportCompletedWaitTypeDef = TypedDict(
     "_OptionalDescribeImportRequestBotImportCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImportRequestBotImportCompletedWaitTypeDef(
     _RequiredDescribeImportRequestBotImportCompletedWaitTypeDef,
     _OptionalDescribeImportRequestBotImportCompletedWaitTypeDef,
 ):
     pass
 
-
 DescribeBotVersionResponseTypeDef = TypedDict(
     "DescribeBotVersionResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "botVersion": str,
         "description": str,
@@ -3414,15 +3445,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
     "UpdateBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
@@ -3442,15 +3473,15 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestSetSummaryTypeDef = TypedDict(
     "TestSetSummaryTypeDef",
     {
         "testSetId": str,
@@ -3476,16 +3507,26 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DialogStateOutputTypeDef = TypedDict(
+    "DialogStateOutputTypeDef",
+    {
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentOverrideOutputTypeDef,
+        "sessionAttributes": Dict[str, str],
     },
+    total=False,
 )
 
 DialogStateTypeDef = TypedDict(
     "DialogStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentOverrideTypeDef,
@@ -3545,15 +3586,15 @@
     "ListImportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "importSummaries": List[ImportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputSessionStateSpecificationTypeDef = TypedDict(
     "InputSessionStateSpecificationTypeDef",
     {
         "sessionAttributes": Dict[str, str],
@@ -3587,31 +3628,29 @@
         "filters": Sequence[IntentFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListIntentsRequestRequestTypeDef(
     _RequiredListIntentsRequestRequestTypeDef, _OptionalListIntentsRequestRequestTypeDef
 ):
     pass
 
-
 ListRecommendedIntentsResponseTypeDef = TypedDict(
     "ListRecommendedIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotTypesRequestRequestTypeDef",
     {
         "botId": str,
@@ -3626,30 +3665,28 @@
         "filters": Sequence[SlotTypeFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListSlotTypesRequestRequestTypeDef(
     _RequiredListSlotTypesRequestRequestTypeDef, _OptionalListSlotTypesRequestRequestTypeDef
 ):
     pass
 
-
 ListSlotTypesResponseTypeDef = TypedDict(
     "ListSlotTypesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "slotTypeSummaries": List[SlotTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSlotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotsRequestRequestTypeDef",
     {
         "botId": str,
@@ -3665,21 +3702,19 @@
         "filters": Sequence[SlotFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListSlotsRequestRequestTypeDef(
     _RequiredListSlotsRequestRequestTypeDef, _OptionalListSlotsRequestRequestTypeDef
 ):
     pass
 
-
 ListTestExecutionsRequestRequestTypeDef = TypedDict(
     "ListTestExecutionsRequestRequestTypeDef",
     {
         "sortBy": TestExecutionSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
@@ -3715,23 +3750,39 @@
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
+SlotTypeValueOutputTypeDef = TypedDict(
+    "SlotTypeValueOutputTypeDef",
+    {
+        "sampleValue": SampleValueTypeDef,
+        "synonyms": List[SampleValueTypeDef],
+    },
+    total=False,
+)
+
 SlotTypeValueTypeDef = TypedDict(
     "SlotTypeValueTypeDef",
     {
         "sampleValue": SampleValueTypeDef,
         "synonyms": Sequence[SampleValueTypeDef],
     },
     total=False,
 )
 
+SlotDefaultValueSpecificationOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecificationOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueTypeDef],
+    },
+)
+
 SlotDefaultValueSpecificationTypeDef = TypedDict(
     "SlotDefaultValueSpecificationTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
@@ -3739,14 +3790,24 @@
     "SlotResolutionTestResultItemTypeDef",
     {
         "slotName": str,
         "resultCounts": SlotResolutionTestResultItemCountsTypeDef,
     },
 )
 
+SlotValueOverrideOutputTypeDef = TypedDict(
+    "SlotValueOverrideOutputTypeDef",
+    {
+        "shape": SlotShapeType,
+        "value": SlotValueTypeDef,
+        "values": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 SlotValueOverrideTypeDef = TypedDict(
     "SlotValueOverrideTypeDef",
     {
         "shape": SlotShapeType,
         "value": SlotValueTypeDef,
         "values": Sequence[Dict[str, Any]],
     },
@@ -3764,21 +3825,19 @@
     {
         "regexFilter": SlotValueRegexFilterTypeDef,
         "advancedRecognitionSetting": AdvancedRecognitionSettingTypeDef,
     },
     total=False,
 )
 
-
 class SlotValueSelectionSettingTypeDef(
     _RequiredSlotValueSelectionSettingTypeDef, _OptionalSlotValueSelectionSettingTypeDef
 ):
     pass
 
-
 TestSetDiscrepancyErrorsTypeDef = TypedDict(
     "TestSetDiscrepancyErrorsTypeDef",
     {
         "intentDiscrepancies": List[TestSetIntentDiscrepancyItemTypeDef],
         "slotDiscrepancies": List[TestSetSlotDiscrepancyItemTypeDef],
     },
 )
@@ -3787,41 +3846,64 @@
     "TestSetDiscrepancyReportResourceTargetTypeDef",
     {
         "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetTypeDef,
     },
     total=False,
 )
 
+_RequiredTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
+    "_RequiredTestSetImportResourceSpecificationOutputTypeDef",
+    {
+        "testSetName": str,
+        "roleArn": str,
+        "storageLocation": TestSetStorageLocationTypeDef,
+        "importInputLocation": TestSetImportInputLocationTypeDef,
+        "modality": TestSetModalityType,
+    },
+)
+_OptionalTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
+    "_OptionalTestSetImportResourceSpecificationOutputTypeDef",
+    {
+        "description": str,
+        "testSetTags": Dict[str, str],
+    },
+    total=False,
+)
+
+class TestSetImportResourceSpecificationOutputTypeDef(
+    _RequiredTestSetImportResourceSpecificationOutputTypeDef,
+    _OptionalTestSetImportResourceSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_RequiredTestSetImportResourceSpecificationTypeDef",
     {
         "testSetName": str,
         "roleArn": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "importInputLocation": TestSetImportInputLocationTypeDef,
         "modality": TestSetModalityType,
     },
 )
 _OptionalTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_OptionalTestSetImportResourceSpecificationTypeDef",
     {
         "description": str,
-        "testSetTags": Dict[str, str],
+        "testSetTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TestSetImportResourceSpecificationTypeDef(
     _RequiredTestSetImportResourceSpecificationTypeDef,
     _OptionalTestSetImportResourceSpecificationTypeDef,
 ):
     pass
 
-
 _RequiredUserTurnOutputSpecificationTypeDef = TypedDict(
     "_RequiredUserTurnOutputSpecificationTypeDef",
     {
         "intent": UserTurnIntentOutputTypeDef,
     },
 )
 _OptionalUserTurnOutputSpecificationTypeDef = TypedDict(
@@ -3829,21 +3911,19 @@
     {
         "activeContexts": List[ActiveContextTypeDef],
         "transcript": str,
     },
     total=False,
 )
 
-
 class UserTurnOutputSpecificationTypeDef(
     _RequiredUserTurnOutputSpecificationTypeDef, _OptionalUserTurnOutputSpecificationTypeDef
 ):
     pass
 
-
 UtteranceInputSpecificationTypeDef = TypedDict(
     "UtteranceInputSpecificationTypeDef",
     {
         "textInput": str,
         "audioInput": UtteranceAudioInputSpecificationTypeDef,
     },
     total=False,
@@ -3861,21 +3941,19 @@
         "allowInterrupt": bool,
         "audioAndDTMFInputSpecification": AudioAndDTMFInputSpecificationTypeDef,
         "textInputSpecification": TextInputSpecificationTypeDef,
     },
     total=False,
 )
 
-
 class PromptAttemptSpecificationTypeDef(
     _RequiredPromptAttemptSpecificationTypeDef, _OptionalPromptAttemptSpecificationTypeDef
 ):
     pass
 
-
 AudioLogSettingTypeDef = TypedDict(
     "AudioLogSettingTypeDef",
     {
         "enabled": bool,
         "destination": AudioLogDestinationTypeDef,
     },
 )
@@ -3889,15 +3967,15 @@
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
         "target": TestExecutionTargetTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartTestExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestExecutionRequestRequestTypeDef",
     {
         "testSetId": str,
@@ -3909,32 +3987,30 @@
     "_OptionalStartTestExecutionRequestRequestTypeDef",
     {
         "testExecutionModality": TestExecutionModalityType,
     },
     total=False,
 )
 
-
 class StartTestExecutionRequestRequestTypeDef(
     _RequiredStartTestExecutionRequestRequestTypeDef,
     _OptionalStartTestExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 StartTestExecutionResponseTypeDef = TypedDict(
     "StartTestExecutionResponseTypeDef",
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestExecutionTargetTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionSummaryTypeDef = TypedDict(
     "TestExecutionSummaryTypeDef",
     {
         "testExecutionId": str,
@@ -3956,14 +4032,25 @@
         "botLocaleExportUrl": str,
         "associatedTranscriptsUrl": str,
         "statistics": BotRecommendationResultStatisticsTypeDef,
     },
     total=False,
 )
 
+MessageOutputTypeDef = TypedDict(
+    "MessageOutputTypeDef",
+    {
+        "plainTextMessage": PlainTextMessageTypeDef,
+        "customPayload": CustomPayloadTypeDef,
+        "ssmlMessage": SSMLMessageTypeDef,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
+    total=False,
+)
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "plainTextMessage": PlainTextMessageTypeDef,
         "customPayload": CustomPayloadTypeDef,
         "ssmlMessage": SSMLMessageTypeDef,
         "imageResponseCard": ImageResponseCardTypeDef,
@@ -3989,21 +4076,22 @@
     "_OptionalBotAliasLocaleSettingsTypeDef",
     {
         "codeHookSpecification": CodeHookSpecificationTypeDef,
     },
     total=False,
 )
 
-
 class BotAliasLocaleSettingsTypeDef(
     _RequiredBotAliasLocaleSettingsTypeDef, _OptionalBotAliasLocaleSettingsTypeDef
 ):
     pass
 
-
+CompositeSlotTypeSettingUnionTypeDef = Union[
+    CompositeSlotTypeSettingTypeDef, CompositeSlotTypeSettingOutputTypeDef
+]
 ConversationLevelTestResultsTypeDef = TypedDict(
     "ConversationLevelTestResultsTypeDef",
     {
         "items": List[ConversationLevelTestResultItemTypeDef],
     },
 )
 
@@ -4019,56 +4107,72 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTestExecutionResultItemsRequestRequestTypeDef(
     _RequiredListTestExecutionResultItemsRequestRequestTypeDef,
     _OptionalListTestExecutionResultItemsRequestRequestTypeDef,
 ):
     pass
 
+TestSetGenerationDataSourceOutputTypeDef = TypedDict(
+    "TestSetGenerationDataSourceOutputTypeDef",
+    {
+        "conversationLogsDataSource": ConversationLogsDataSourceOutputTypeDef,
+    },
+    total=False,
+)
 
-TestSetGenerationDataSourceTypeDef = TypedDict(
-    "TestSetGenerationDataSourceTypeDef",
+ConversationLogsDataSourceTypeDef = TypedDict(
+    "ConversationLogsDataSourceTypeDef",
     {
-        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "filter": ConversationLogsDataSourceFilterByTypeDef,
+    },
+)
+
+LexTranscriptFilterTypeDef = TypedDict(
+    "LexTranscriptFilterTypeDef",
+    {
+        "dateRangeFilter": DateRangeFilterTypeDef,
     },
     total=False,
 )
 
 ListIntentsResponseTypeDef = TypedDict(
     "ListIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TranscriptFilterTypeDef = TypedDict(
-    "TranscriptFilterTypeDef",
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
-        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
+        "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
     },
     total=False,
 )
 
 ListTestSetsResponseTypeDef = TypedDict(
     "ListTestSetsResponseTypeDef",
     {
         "testSets": List[TestSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExportRequestRequestTypeDef",
     {
         "resourceSpecification": ExportResourceSpecificationTypeDef,
@@ -4079,45 +4183,43 @@
     "_OptionalCreateExportRequestRequestTypeDef",
     {
         "filePassword": str,
     },
     total=False,
 )
 
-
 class CreateExportRequestRequestTypeDef(
     _RequiredCreateExportRequestRequestTypeDef, _OptionalCreateExportRequestRequestTypeDef
 ):
     pass
 
-
 CreateExportResponseTypeDef = TypedDict(
     "CreateExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportResponseTypeDef = TypedDict(
     "DescribeExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "failureReasons": List[str],
         "downloadUrl": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "exportId": str,
@@ -4135,15 +4237,15 @@
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExternalSourceSettingTypeDef = TypedDict(
     "ExternalSourceSettingTypeDef",
     {
         "grammarSlotTypeSetting": GrammarSlotTypeSettingTypeDef,
@@ -4175,39 +4277,38 @@
         "filters": Sequence[AggregatedUtterancesFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListAggregatedUtterancesRequestRequestTypeDef(
     _RequiredListAggregatedUtterancesRequestRequestTypeDef,
     _OptionalListAggregatedUtterancesRequestRequestTypeDef,
 ):
     pass
 
-
 ListAggregatedUtterancesResponseTypeDef = TypedDict(
     "ListAggregatedUtterancesResponseTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "botVersion": str,
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationTypeDef,
         "aggregationWindowStartTime": datetime,
         "aggregationWindowEndTime": datetime,
         "aggregationLastRefreshedDateTime": datetime,
         "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SlotTypeValueUnionTypeDef = Union[SlotTypeValueTypeDef, SlotTypeValueOutputTypeDef]
 IntentLevelSlotResolutionTestResultItemTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
         "slotResolutionResults": List[SlotResolutionTestResultItemTypeDef],
     },
@@ -4224,15 +4325,15 @@
 CreateTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestSetDiscrepancyReportResourceTargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
@@ -4240,16 +4341,27 @@
         "creationDateTime": datetime,
         "target": TestSetDiscrepancyReportResourceTargetTypeDef,
         "testSetDiscrepancyReportStatus": TestSetDiscrepancyReportStatusType,
         "lastUpdatedDataTime": datetime,
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportResourceSpecificationOutputTypeDef = TypedDict(
+    "ImportResourceSpecificationOutputTypeDef",
+    {
+        "botImportSpecification": BotImportSpecificationOutputTypeDef,
+        "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
+        "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
+        "testSetImportResourceSpecification": TestSetImportResourceSpecificationOutputTypeDef,
     },
+    total=False,
 )
 
 ImportResourceSpecificationTypeDef = TypedDict(
     "ImportResourceSpecificationTypeDef",
     {
         "botImportSpecification": BotImportSpecificationTypeDef,
         "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
@@ -4270,48 +4382,72 @@
     {
         "requestAttributes": Dict[str, str],
         "sessionState": InputSessionStateSpecificationTypeDef,
     },
     total=False,
 )
 
-
 class UserTurnInputSpecificationTypeDef(
     _RequiredUserTurnInputSpecificationTypeDef, _OptionalUserTurnInputSpecificationTypeDef
 ):
     pass
 
-
 ListTestExecutionsResponseTypeDef = TypedDict(
     "ListTestExecutionsResponseTypeDef",
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredMessageGroupOutputTypeDef = TypedDict(
+    "_RequiredMessageGroupOutputTypeDef",
+    {
+        "message": MessageOutputTypeDef,
+    },
+)
+_OptionalMessageGroupOutputTypeDef = TypedDict(
+    "_OptionalMessageGroupOutputTypeDef",
+    {
+        "variations": List[MessageOutputTypeDef],
+    },
+    total=False,
+)
+
+class MessageGroupOutputTypeDef(
+    _RequiredMessageGroupOutputTypeDef, _OptionalMessageGroupOutputTypeDef
+):
+    pass
+
 _RequiredMessageGroupTypeDef = TypedDict(
     "_RequiredMessageGroupTypeDef",
     {
         "message": MessageTypeDef,
     },
 )
 _OptionalMessageGroupTypeDef = TypedDict(
     "_OptionalMessageGroupTypeDef",
     {
         "variations": Sequence[MessageTypeDef],
     },
     total=False,
 )
 
-
 class MessageGroupTypeDef(_RequiredMessageGroupTypeDef, _OptionalMessageGroupTypeDef):
     pass
 
+ConversationLogSettingsOutputTypeDef = TypedDict(
+    "ConversationLogSettingsOutputTypeDef",
+    {
+        "textLogSettings": List[TextLogSettingTypeDef],
+        "audioLogSettings": List[AudioLogSettingTypeDef],
+    },
+    total=False,
+)
 
 ConversationLogSettingsTypeDef = TypedDict(
     "ConversationLogSettingsTypeDef",
     {
         "textLogSettings": Sequence[TextLogSettingTypeDef],
         "audioLogSettings": Sequence[AudioLogSettingTypeDef],
     },
@@ -4324,241 +4460,240 @@
         "testSetGenerationId": str,
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "failureReasons": List[str],
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
+StartTestSetGenerationResponseTypeDef = TypedDict(
+    "StartTestSetGenerationResponseTypeDef",
     {
+        "testSetGenerationId": str,
+        "creationDateTime": datetime,
+        "testSetGenerationStatus": TestSetGenerationStatusType,
         "testSetName": str,
+        "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
+        "testSetTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
+
+TestSetGenerationDataSourceTypeDef = TypedDict(
+    "TestSetGenerationDataSourceTypeDef",
     {
-        "description": str,
-        "testSetTags": Mapping[str, str],
+        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
     },
     total=False,
 )
 
-
-class StartTestSetGenerationRequestRequestTypeDef(
-    _RequiredStartTestSetGenerationRequestRequestTypeDef,
-    _OptionalStartTestSetGenerationRequestRequestTypeDef,
-):
-    pass
-
-
-StartTestSetGenerationResponseTypeDef = TypedDict(
-    "StartTestSetGenerationResponseTypeDef",
+TranscriptFilterTypeDef = TypedDict(
+    "TranscriptFilterTypeDef",
     {
-        "testSetGenerationId": str,
-        "creationDateTime": datetime,
-        "testSetGenerationStatus": TestSetGenerationStatusType,
-        "testSetName": str,
-        "description": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
-        "roleArn": str,
-        "testSetTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
     },
+    total=False,
 )
 
-_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_RequiredS3BucketTranscriptSourceTypeDef",
+_RequiredS3BucketTranscriptSourceOutputTypeDef = TypedDict(
+    "_RequiredS3BucketTranscriptSourceOutputTypeDef",
     {
         "s3BucketName": str,
         "transcriptFormat": Literal["Lex"],
     },
 )
-_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_OptionalS3BucketTranscriptSourceTypeDef",
+_OptionalS3BucketTranscriptSourceOutputTypeDef = TypedDict(
+    "_OptionalS3BucketTranscriptSourceOutputTypeDef",
     {
-        "pathFormat": PathFormatTypeDef,
-        "transcriptFilter": TranscriptFilterTypeDef,
+        "pathFormat": PathFormatOutputTypeDef,
+        "transcriptFilter": TranscriptFilterOutputTypeDef,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
-class S3BucketTranscriptSourceTypeDef(
-    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
+class S3BucketTranscriptSourceOutputTypeDef(
+    _RequiredS3BucketTranscriptSourceOutputTypeDef, _OptionalS3BucketTranscriptSourceOutputTypeDef
 ):
     pass
 
-
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotTypeRequestRequestTypeDef",
+CreateSlotTypeResponseTypeDef = TypedDict(
+    "CreateSlotTypeResponseTypeDef",
     {
+        "slotTypeId": str,
         "slotTypeName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotTypeRequestRequestTypeDef",
-    {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateSlotTypeRequestRequestTypeDef(
-    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
-):
-    pass
-
-
-CreateSlotTypeResponseTypeDef = TypedDict(
-    "CreateSlotTypeResponseTypeDef",
+DescribeSlotTypeResponseTypeDef = TypedDict(
+    "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSlotTypeResponseTypeDef = TypedDict(
-    "DescribeSlotTypeResponseTypeDef",
+UpdateSlotTypeResponseTypeDef = TypedDict(
+    "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
+_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
-        "slotTypeId": str,
         "slotTypeName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
     total=False,
 )
 
-
-class UpdateSlotTypeRequestRequestTypeDef(
-    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+class CreateSlotTypeRequestRequestTypeDef(
+    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
 ):
     pass
 
-
-UpdateSlotTypeResponseTypeDef = TypedDict(
-    "UpdateSlotTypeResponseTypeDef",
+_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
-        "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateSlotTypeRequestRequestTypeDef(
+    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+):
+    pass
+
 IntentLevelSlotResolutionTestResultsTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultsTypeDef",
     {
         "items": List[IntentLevelSlotResolutionTestResultItemTypeDef],
     },
 )
 
 DescribeImportResponseTypeDef = TypedDict(
     "DescribeImportResponseTypeDef",
     {
         "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
+    {
+        "importId": str,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
+        "mergeStrategy": MergeStrategyType,
+        "importStatus": ImportStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportResourceSpecificationUnionTypeDef = Union[
+    ImportResourceSpecificationTypeDef, ImportResourceSpecificationOutputTypeDef
+]
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationTypeDef,
         "mergeStrategy": MergeStrategyType,
     },
@@ -4567,33 +4702,19 @@
     "_OptionalStartImportRequestRequestTypeDef",
     {
         "filePassword": str,
     },
     total=False,
 )
 
-
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
-
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
-    {
-        "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
-        "mergeStrategy": MergeStrategyType,
-        "importStatus": ImportStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUserTurnResultTypeDef = TypedDict(
     "_RequiredUserTurnResultTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expectedOutput": UserTurnOutputSpecificationTypeDef,
     },
 )
@@ -4607,27 +4728,130 @@
         "slotMatchResult": TestResultMatchStatusType,
         "speechTranscriptionResult": TestResultMatchStatusType,
         "conversationLevelResult": ConversationLevelResultDetailTypeDef,
     },
     total=False,
 )
 
-
 class UserTurnResultTypeDef(_RequiredUserTurnResultTypeDef, _OptionalUserTurnResultTypeDef):
     pass
 
-
 UserTurnSpecificationTypeDef = TypedDict(
     "UserTurnSpecificationTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expected": UserTurnOutputSpecificationTypeDef,
     },
 )
 
+_RequiredFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentStartResponseSpecificationOutputTypeDef",
+    {
+        "delayInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+    },
+)
+_OptionalFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentStartResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+class FulfillmentStartResponseSpecificationOutputTypeDef(
+    _RequiredFulfillmentStartResponseSpecificationOutputTypeDef,
+    _OptionalFulfillmentStartResponseSpecificationOutputTypeDef,
+):
+    pass
+
+_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef",
+    {
+        "frequencyInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+    },
+)
+_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+class FulfillmentUpdateResponseSpecificationOutputTypeDef(
+    _RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef,
+    _OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef,
+):
+    pass
+
+_RequiredPromptSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPromptSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "maxRetries": int,
+    },
+)
+_OptionalPromptSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPromptSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+        "messageSelectionStrategy": MessageSelectionStrategyType,
+        "promptAttemptsSpecification": Dict[PromptAttemptType, PromptAttemptSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class PromptSpecificationOutputTypeDef(
+    _RequiredPromptSpecificationOutputTypeDef, _OptionalPromptSpecificationOutputTypeDef
+):
+    pass
+
+_RequiredResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+    },
+)
+_OptionalResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+class ResponseSpecificationOutputTypeDef(
+    _RequiredResponseSpecificationOutputTypeDef, _OptionalResponseSpecificationOutputTypeDef
+):
+    pass
+
+_RequiredStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredStillWaitingResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "frequencyInSeconds": int,
+        "timeoutInSeconds": int,
+    },
+)
+_OptionalStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalStillWaitingResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+class StillWaitingResponseSpecificationOutputTypeDef(
+    _RequiredStillWaitingResponseSpecificationOutputTypeDef,
+    _OptionalStillWaitingResponseSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4635,22 +4859,20 @@
     "_OptionalFulfillmentStartResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
-
 class FulfillmentStartResponseSpecificationTypeDef(
     _RequiredFulfillmentStartResponseSpecificationTypeDef,
     _OptionalFulfillmentStartResponseSpecificationTypeDef,
 ):
     pass
 
-
 _RequiredFulfillmentUpdateResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentUpdateResponseSpecificationTypeDef",
     {
         "frequencyInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4658,22 +4880,20 @@
     "_OptionalFulfillmentUpdateResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
-
 class FulfillmentUpdateResponseSpecificationTypeDef(
     _RequiredFulfillmentUpdateResponseSpecificationTypeDef,
     _OptionalFulfillmentUpdateResponseSpecificationTypeDef,
 ):
     pass
 
-
 _RequiredPromptSpecificationTypeDef = TypedDict(
     "_RequiredPromptSpecificationTypeDef",
     {
         "messageGroups": Sequence[MessageGroupTypeDef],
         "maxRetries": int,
     },
 )
@@ -4685,42 +4905,38 @@
         "promptAttemptsSpecification": Mapping[
             PromptAttemptType, PromptAttemptSpecificationTypeDef
         ],
     },
     total=False,
 )
 
-
 class PromptSpecificationTypeDef(
     _RequiredPromptSpecificationTypeDef, _OptionalPromptSpecificationTypeDef
 ):
     pass
 
-
 _RequiredResponseSpecificationTypeDef = TypedDict(
     "_RequiredResponseSpecificationTypeDef",
     {
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
 _OptionalResponseSpecificationTypeDef = TypedDict(
     "_OptionalResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
-
 class ResponseSpecificationTypeDef(
     _RequiredResponseSpecificationTypeDef, _OptionalResponseSpecificationTypeDef
 ):
     pass
 
-
 _RequiredStillWaitingResponseSpecificationTypeDef = TypedDict(
     "_RequiredStillWaitingResponseSpecificationTypeDef",
     {
         "messageGroups": Sequence[MessageGroupTypeDef],
         "frequencyInSeconds": int,
         "timeoutInSeconds": int,
     },
@@ -4729,86 +4945,103 @@
     "_OptionalStillWaitingResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
-
 class StillWaitingResponseSpecificationTypeDef(
     _RequiredStillWaitingResponseSpecificationTypeDef,
     _OptionalStillWaitingResponseSpecificationTypeDef,
 ):
     pass
 
-
-_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotAliasRequestRequestTypeDef",
+CreateBotAliasResponseTypeDef = TypedDict(
+    "CreateBotAliasResponseTypeDef",
     {
+        "botAliasId": str,
         "botAliasName": str,
-        "botId": str,
-    },
-)
-_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotAliasRequestRequestTypeDef",
-    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "tags": Mapping[str, str],
+        "botAliasStatus": BotAliasStatusType,
+        "botId": str,
+        "creationDateTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateBotAliasRequestRequestTypeDef(
-    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
-):
-    pass
-
-
-CreateBotAliasResponseTypeDef = TypedDict(
-    "CreateBotAliasResponseTypeDef",
+DescribeBotAliasResponseTypeDef = TypedDict(
+    "DescribeBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "lastUpdatedDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBotAliasResponseTypeDef = TypedDict(
-    "DescribeBotAliasResponseTypeDef",
+UpdateBotAliasResponseTypeDef = TypedDict(
+    "UpdateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "parentBotNetworks": List[ParentBotNetworkTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConversationLogSettingsUnionTypeDef = Union[
+    ConversationLogSettingsTypeDef, ConversationLogSettingsOutputTypeDef
+]
+_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotAliasRequestRequestTypeDef",
+    {
+        "botAliasName": str,
+        "botId": str,
     },
 )
+_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotAliasRequestRequestTypeDef",
+    {
+        "description": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateBotAliasRequestRequestTypeDef(
+    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
+):
+    pass
 
 _RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "botId": str,
@@ -4822,43 +5055,72 @@
         "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBotAliasRequestRequestTypeDef(
     _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
 ):
     pass
 
-
-UpdateBotAliasResponseTypeDef = TypedDict(
-    "UpdateBotAliasResponseTypeDef",
+_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
+    {
+        "testSetName": str,
+        "storageLocation": TestSetStorageLocationTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "roleArn": str,
+    },
+)
+_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
     {
-        "botAliasId": str,
-        "botAliasName": str,
         "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasStatus": BotAliasStatusType,
-        "botId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "testSetTags": Mapping[str, str],
     },
+    total=False,
 )
 
-TranscriptSourceSettingTypeDef = TypedDict(
-    "TranscriptSourceSettingTypeDef",
+class StartTestSetGenerationRequestRequestTypeDef(
+    _RequiredStartTestSetGenerationRequestRequestTypeDef,
+    _OptionalStartTestSetGenerationRequestRequestTypeDef,
+):
+    pass
+
+TestSetGenerationDataSourceUnionTypeDef = Union[
+    TestSetGenerationDataSourceTypeDef, TestSetGenerationDataSourceOutputTypeDef
+]
+_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_RequiredS3BucketTranscriptSourceTypeDef",
     {
-        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
+        "s3BucketName": str,
+        "transcriptFormat": Literal["Lex"],
+    },
+)
+_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_OptionalS3BucketTranscriptSourceTypeDef",
+    {
+        "pathFormat": PathFormatTypeDef,
+        "transcriptFilter": TranscriptFilterTypeDef,
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+class S3BucketTranscriptSourceTypeDef(
+    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
+):
+    pass
+
+TranscriptSourceSettingOutputTypeDef = TypedDict(
+    "TranscriptSourceSettingOutputTypeDef",
+    {
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceOutputTypeDef,
     },
     total=False,
 )
 
 TestSetTurnResultTypeDef = TypedDict(
     "TestSetTurnResultTypeDef",
     {
@@ -4873,51 +5135,123 @@
     {
         "agentTurn": AgentTurnSpecificationTypeDef,
         "userTurn": UserTurnSpecificationTypeDef,
     },
     total=False,
 )
 
-_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
+_RequiredFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdatesSpecificationOutputTypeDef",
     {
         "active": bool,
     },
 )
-_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
+_OptionalFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdatesSpecificationOutputTypeDef",
     {
-        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
-        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
+        "startResponse": FulfillmentStartResponseSpecificationOutputTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationOutputTypeDef,
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
-
-class FulfillmentUpdatesSpecificationTypeDef(
-    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
+class FulfillmentUpdatesSpecificationOutputTypeDef(
+    _RequiredFulfillmentUpdatesSpecificationOutputTypeDef,
+    _OptionalFulfillmentUpdatesSpecificationOutputTypeDef,
 ):
     pass
 
-
 SlotSummaryTypeDef = TypedDict(
     "SlotSummaryTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotConstraint": SlotConstraintType,
         "slotTypeId": str,
-        "valueElicitationPromptSpecification": PromptSpecificationTypeDef,
+        "valueElicitationPromptSpecification": PromptSpecificationOutputTypeDef,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+_RequiredConditionalBranchOutputTypeDef = TypedDict(
+    "_RequiredConditionalBranchOutputTypeDef",
+    {
+        "name": str,
+        "condition": ConditionTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+    },
+)
+_OptionalConditionalBranchOutputTypeDef = TypedDict(
+    "_OptionalConditionalBranchOutputTypeDef",
+    {
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ConditionalBranchOutputTypeDef(
+    _RequiredConditionalBranchOutputTypeDef, _OptionalConditionalBranchOutputTypeDef
+):
+    pass
+
+DefaultConditionalBranchOutputTypeDef = TypedDict(
+    "DefaultConditionalBranchOutputTypeDef",
+    {
+        "nextStep": DialogStateOutputTypeDef,
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredWaitAndContinueSpecificationOutputTypeDef = TypedDict(
+    "_RequiredWaitAndContinueSpecificationOutputTypeDef",
+    {
+        "waitingResponse": ResponseSpecificationOutputTypeDef,
+        "continueResponse": ResponseSpecificationOutputTypeDef,
+    },
+)
+_OptionalWaitAndContinueSpecificationOutputTypeDef = TypedDict(
+    "_OptionalWaitAndContinueSpecificationOutputTypeDef",
+    {
+        "stillWaitingResponse": StillWaitingResponseSpecificationOutputTypeDef,
+        "active": bool,
+    },
+    total=False,
+)
+
+class WaitAndContinueSpecificationOutputTypeDef(
+    _RequiredWaitAndContinueSpecificationOutputTypeDef,
+    _OptionalWaitAndContinueSpecificationOutputTypeDef,
+):
+    pass
+
+_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
+    {
+        "active": bool,
+    },
+)
+_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
+    {
+        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
+        "timeoutInSeconds": int,
+    },
+    total=False,
+)
+
+class FulfillmentUpdatesSpecificationTypeDef(
+    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
+):
+    pass
+
 _RequiredConditionalBranchTypeDef = TypedDict(
     "_RequiredConditionalBranchTypeDef",
     {
         "name": str,
         "condition": ConditionTypeDef,
         "nextStep": DialogStateTypeDef,
     },
@@ -4926,21 +5260,19 @@
     "_OptionalConditionalBranchTypeDef",
     {
         "response": ResponseSpecificationTypeDef,
     },
     total=False,
 )
 
-
 class ConditionalBranchTypeDef(
     _RequiredConditionalBranchTypeDef, _OptionalConditionalBranchTypeDef
 ):
     pass
 
-
 DefaultConditionalBranchTypeDef = TypedDict(
     "DefaultConditionalBranchTypeDef",
     {
         "nextStep": DialogStateTypeDef,
         "response": ResponseSpecificationTypeDef,
     },
     total=False,
@@ -4958,92 +5290,73 @@
     {
         "stillWaitingResponse": StillWaitingResponseSpecificationTypeDef,
         "active": bool,
     },
     total=False,
 )
 
-
 class WaitAndContinueSpecificationTypeDef(
     _RequiredWaitAndContinueSpecificationTypeDef, _OptionalWaitAndContinueSpecificationTypeDef
 ):
     pass
 
+TranscriptSourceSettingTypeDef = TypedDict(
+    "TranscriptSourceSettingTypeDef",
+    {
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
+    },
+    total=False,
+)
 
 DescribeBotRecommendationResponseTypeDef = TypedDict(
     "DescribeBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartBotRecommendationRequestRequestTypeDef",
-    {
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class StartBotRecommendationRequestRequestTypeDef(
-    _RequiredStartBotRecommendationRequestRequestTypeDef,
-    _OptionalStartBotRecommendationRequestRequestTypeDef,
-):
-    pass
-
 
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUtteranceLevelTestResultItemTypeDef = TypedDict(
     "_RequiredUtteranceLevelTestResultItemTypeDef",
     {
         "recordNumber": int,
@@ -5054,21 +5367,19 @@
     "_OptionalUtteranceLevelTestResultItemTypeDef",
     {
         "conversationId": str,
     },
     total=False,
 )
 
-
 class UtteranceLevelTestResultItemTypeDef(
     _RequiredUtteranceLevelTestResultItemTypeDef, _OptionalUtteranceLevelTestResultItemTypeDef
 ):
     pass
 
-
 _RequiredTestSetTurnRecordTypeDef = TypedDict(
     "_RequiredTestSetTurnRecordTypeDef",
     {
         "recordNumber": int,
         "turnSpecification": TurnSpecificationTypeDef,
     },
 )
@@ -5077,34 +5388,63 @@
     {
         "conversationId": str,
         "turnNumber": int,
     },
     total=False,
 )
 
-
 class TestSetTurnRecordTypeDef(
     _RequiredTestSetTurnRecordTypeDef, _OptionalTestSetTurnRecordTypeDef
 ):
     pass
 
-
 ListSlotsResponseTypeDef = TypedDict(
     "ListSlotsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConditionalSpecificationOutputTypeDef = TypedDict(
+    "ConditionalSpecificationOutputTypeDef",
+    {
+        "active": bool,
+        "conditionalBranches": List[ConditionalBranchOutputTypeDef],
+        "defaultBranch": DefaultConditionalBranchOutputTypeDef,
+    },
+)
+
+_RequiredSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_RequiredSubSlotValueElicitationSettingOutputTypeDef",
+    {
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+    },
+)
+_OptionalSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_OptionalSubSlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+class SubSlotValueElicitationSettingOutputTypeDef(
+    _RequiredSubSlotValueElicitationSettingOutputTypeDef,
+    _OptionalSubSlotValueElicitationSettingOutputTypeDef,
+):
+    pass
+
 ConditionalSpecificationTypeDef = TypedDict(
     "ConditionalSpecificationTypeDef",
     {
         "active": bool,
         "conditionalBranches": Sequence[ConditionalBranchTypeDef],
         "defaultBranch": DefaultConditionalBranchTypeDef,
     },
@@ -5122,34 +5462,109 @@
         "defaultValueSpecification": SlotDefaultValueSpecificationTypeDef,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "waitAndContinueSpecification": WaitAndContinueSpecificationTypeDef,
     },
     total=False,
 )
 
-
 class SubSlotValueElicitationSettingTypeDef(
     _RequiredSubSlotValueElicitationSettingTypeDef, _OptionalSubSlotValueElicitationSettingTypeDef
 ):
     pass
 
+_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartBotRecommendationRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+    },
+)
+_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartBotRecommendationRequestRequestTypeDef",
+    {
+        "encryptionSetting": EncryptionSettingTypeDef,
+    },
+    total=False,
+)
+
+class StartBotRecommendationRequestRequestTypeDef(
+    _RequiredStartBotRecommendationRequestRequestTypeDef,
+    _OptionalStartBotRecommendationRequestRequestTypeDef,
+):
+    pass
 
+TranscriptSourceSettingUnionTypeDef = Union[
+    TranscriptSourceSettingTypeDef, TranscriptSourceSettingOutputTypeDef
+]
 UtteranceLevelTestResultsTypeDef = TypedDict(
     "UtteranceLevelTestResultsTypeDef",
     {
         "items": List[UtteranceLevelTestResultItemTypeDef],
     },
 )
 
 ListTestSetRecordsResponseTypeDef = TypedDict(
     "ListTestSetRecordsResponseTypeDef",
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IntentClosingSettingOutputTypeDef = TypedDict(
+    "IntentClosingSettingOutputTypeDef",
+    {
+        "closingResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+PostDialogCodeHookInvocationSpecificationOutputTypeDef = TypedDict(
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+PostFulfillmentStatusSpecificationOutputTypeDef = TypedDict(
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+SpecificationsOutputTypeDef = TypedDict(
+    "SpecificationsOutputTypeDef",
+    {
+        "slotTypeId": str,
+        "valueElicitationSetting": SubSlotValueElicitationSettingOutputTypeDef,
     },
 )
 
 IntentClosingSettingTypeDef = TypedDict(
     "IntentClosingSettingTypeDef",
     {
         "closingResponse": ResponseSpecificationTypeDef,
@@ -5208,14 +5623,70 @@
         "intentClassificationTestResults": IntentClassificationTestResultsTypeDef,
         "intentLevelSlotResolutionTestResults": IntentLevelSlotResolutionTestResultsTypeDef,
         "utteranceLevelTestResults": UtteranceLevelTestResultsTypeDef,
     },
     total=False,
 )
 
+_RequiredDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "_RequiredDialogCodeHookInvocationSettingOutputTypeDef",
+    {
+        "enableCodeHookInvocation": bool,
+        "active": bool,
+        "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    },
+)
+_OptionalDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "_OptionalDialogCodeHookInvocationSettingOutputTypeDef",
+    {
+        "invocationLabel": str,
+    },
+    total=False,
+)
+
+class DialogCodeHookInvocationSettingOutputTypeDef(
+    _RequiredDialogCodeHookInvocationSettingOutputTypeDef,
+    _OptionalDialogCodeHookInvocationSettingOutputTypeDef,
+):
+    pass
+
+_RequiredFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentCodeHookSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentCodeHookSettingsOutputTypeDef",
+    {
+        "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationOutputTypeDef,
+        "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationOutputTypeDef,
+        "active": bool,
+    },
+    total=False,
+)
+
+class FulfillmentCodeHookSettingsOutputTypeDef(
+    _RequiredFulfillmentCodeHookSettingsOutputTypeDef,
+    _OptionalFulfillmentCodeHookSettingsOutputTypeDef,
+):
+    pass
+
+SubSlotSettingOutputTypeDef = TypedDict(
+    "SubSlotSettingOutputTypeDef",
+    {
+        "expression": str,
+        "slotSpecifications": Dict[str, SpecificationsOutputTypeDef],
+    },
+    total=False,
+)
+
+IntentClosingSettingUnionTypeDef = Union[
+    IntentClosingSettingTypeDef, IntentClosingSettingOutputTypeDef
+]
 _RequiredDialogCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredDialogCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
         "active": bool,
         "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationTypeDef,
     },
@@ -5224,21 +5695,19 @@
     "_OptionalDialogCodeHookInvocationSettingTypeDef",
     {
         "invocationLabel": str,
     },
     total=False,
 )
 
-
 class DialogCodeHookInvocationSettingTypeDef(
     _RequiredDialogCodeHookInvocationSettingTypeDef, _OptionalDialogCodeHookInvocationSettingTypeDef
 ):
     pass
 
-
 _RequiredFulfillmentCodeHookSettingsTypeDef = TypedDict(
     "_RequiredFulfillmentCodeHookSettingsTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalFulfillmentCodeHookSettingsTypeDef = TypedDict(
@@ -5247,38 +5716,92 @@
         "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationTypeDef,
         "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationTypeDef,
         "active": bool,
     },
     total=False,
 )
 
-
 class FulfillmentCodeHookSettingsTypeDef(
     _RequiredFulfillmentCodeHookSettingsTypeDef, _OptionalFulfillmentCodeHookSettingsTypeDef
 ):
     pass
 
-
 SubSlotSettingTypeDef = TypedDict(
     "SubSlotSettingTypeDef",
     {
         "expression": str,
         "slotSpecifications": Mapping[str, SpecificationsTypeDef],
     },
     total=False,
 )
 
 ListTestExecutionResultItemsResponseTypeDef = TypedDict(
     "ListTestExecutionResultItemsResponseTypeDef",
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitialResponseSettingOutputTypeDef = TypedDict(
+    "InitialResponseSettingOutputTypeDef",
+    {
+        "initialResponse": ResponseSpecificationOutputTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredIntentConfirmationSettingOutputTypeDef = TypedDict(
+    "_RequiredIntentConfirmationSettingOutputTypeDef",
+    {
+        "promptSpecification": PromptSpecificationOutputTypeDef,
     },
 )
+_OptionalIntentConfirmationSettingOutputTypeDef = TypedDict(
+    "_OptionalIntentConfirmationSettingOutputTypeDef",
+    {
+        "declinationResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "confirmationResponse": ResponseSpecificationOutputTypeDef,
+        "confirmationNextStep": DialogStateOutputTypeDef,
+        "confirmationConditional": ConditionalSpecificationOutputTypeDef,
+        "declinationNextStep": DialogStateOutputTypeDef,
+        "declinationConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
+    },
+    total=False,
+)
+
+class IntentConfirmationSettingOutputTypeDef(
+    _RequiredIntentConfirmationSettingOutputTypeDef, _OptionalIntentConfirmationSettingOutputTypeDef
+):
+    pass
+
+SlotCaptureSettingOutputTypeDef = TypedDict(
+    "SlotCaptureSettingOutputTypeDef",
+    {
+        "captureResponse": ResponseSpecificationOutputTypeDef,
+        "captureNextStep": DialogStateOutputTypeDef,
+        "captureConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
+    },
+    total=False,
+)
 
 InitialResponseSettingTypeDef = TypedDict(
     "InitialResponseSettingTypeDef",
     {
         "initialResponse": ResponseSpecificationTypeDef,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
@@ -5308,21 +5831,19 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-
 class IntentConfirmationSettingTypeDef(
     _RequiredIntentConfirmationSettingTypeDef, _OptionalIntentConfirmationSettingTypeDef
 ):
     pass
 
-
 SlotCaptureSettingTypeDef = TypedDict(
     "SlotCaptureSettingTypeDef",
     {
         "captureResponse": ResponseSpecificationTypeDef,
         "captureNextStep": DialogStateTypeDef,
         "captureConditional": ConditionalSpecificationTypeDef,
         "failureResponse": ResponseSpecificationTypeDef,
@@ -5330,160 +5851,190 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIntentRequestRequestTypeDef",
+FulfillmentCodeHookSettingsUnionTypeDef = Union[
+    FulfillmentCodeHookSettingsTypeDef, FulfillmentCodeHookSettingsOutputTypeDef
+]
+SubSlotSettingUnionTypeDef = Union[SubSlotSettingTypeDef, SubSlotSettingOutputTypeDef]
+CreateIntentResponseTypeDef = TypedDict(
+    "CreateIntentResponseTypeDef",
     {
+        "intentId": str,
         "intentName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIntentRequestRequestTypeDef",
-    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
+        "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": Sequence[InputContextTypeDef],
-        "outputContexts": Sequence[OutputContextTypeDef],
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateIntentRequestRequestTypeDef(
-    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
-):
-    pass
-
-
-CreateIntentResponseTypeDef = TypedDict(
-    "CreateIntentResponseTypeDef",
+DescribeIntentResponseTypeDef = TypedDict(
+    "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "slotPriorities": List[SlotPriorityTypeDef],
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "lastUpdatedDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeIntentResponseTypeDef = TypedDict(
-    "DescribeIntentResponseTypeDef",
+UpdateIntentResponseTypeDef = TypedDict(
+    "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
         "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIntentRequestRequestTypeDef",
+_RequiredSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_RequiredSlotValueElicitationSettingOutputTypeDef",
+    {
+        "slotConstraint": SlotConstraintType,
+    },
+)
+_OptionalSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_OptionalSlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+        "slotCaptureSetting": SlotCaptureSettingOutputTypeDef,
+    },
+    total=False,
+)
+
+class SlotValueElicitationSettingOutputTypeDef(
+    _RequiredSlotValueElicitationSettingOutputTypeDef,
+    _OptionalSlotValueElicitationSettingOutputTypeDef,
+):
+    pass
+
+InitialResponseSettingUnionTypeDef = Union[
+    InitialResponseSettingTypeDef, InitialResponseSettingOutputTypeDef
+]
+_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIntentRequestRequestTypeDef",
     {
-        "intentId": str,
         "intentName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIntentRequestRequestTypeDef",
+_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIntentRequestRequestTypeDef",
     {
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "initialResponseSetting": InitialResponseSettingTypeDef,
     },
     total=False,
 )
 
-
-class UpdateIntentRequestRequestTypeDef(
-    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+class CreateIntentRequestRequestTypeDef(
+    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
 ):
     pass
 
-
-UpdateIntentResponseTypeDef = TypedDict(
-    "UpdateIntentResponseTypeDef",
+IntentConfirmationSettingUnionTypeDef = Union[
+    IntentConfirmationSettingTypeDef, IntentConfirmationSettingOutputTypeDef
+]
+_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "intentName": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIntentRequestRequestTypeDef",
+    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
+        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "inputContexts": Sequence[InputContextTypeDef],
+        "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateIntentRequestRequestTypeDef(
+    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+):
+    pass
+
 _RequiredSlotValueElicitationSettingTypeDef = TypedDict(
     "_RequiredSlotValueElicitationSettingTypeDef",
     {
         "slotConstraint": SlotConstraintType,
     },
 )
 _OptionalSlotValueElicitationSettingTypeDef = TypedDict(
@@ -5494,136 +6045,133 @@
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "waitAndContinueSpecification": WaitAndContinueSpecificationTypeDef,
         "slotCaptureSetting": SlotCaptureSettingTypeDef,
     },
     total=False,
 )
 
-
 class SlotValueElicitationSettingTypeDef(
     _RequiredSlotValueElicitationSettingTypeDef, _OptionalSlotValueElicitationSettingTypeDef
 ):
     pass
 
-
-_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotRequestRequestTypeDef",
+CreateSlotResponseTypeDef = TypedDict(
+    "CreateSlotResponseTypeDef",
     {
+        "slotId": str,
         "slotName": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "description": str,
+        "slotTypeId": str,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-    },
-)
-_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeId": str,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "creationDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateSlotRequestRequestTypeDef(
-    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
-):
-    pass
-
-
-CreateSlotResponseTypeDef = TypedDict(
-    "CreateSlotResponseTypeDef",
+DescribeSlotResponseTypeDef = TypedDict(
+    "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSlotResponseTypeDef = TypedDict(
-    "DescribeSlotResponseTypeDef",
+UpdateSlotResponseTypeDef = TypedDict(
+    "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotRequestRequestTypeDef",
+_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotRequestRequestTypeDef",
     {
-        "slotId": str,
         "slotName": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
     },
 )
-_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotRequestRequestTypeDef",
+_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeId": str,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
     },
     total=False,
 )
 
-
-class UpdateSlotRequestRequestTypeDef(
-    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+class CreateSlotRequestRequestTypeDef(
+    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
 ):
     pass
 
-
-UpdateSlotResponseTypeDef = TypedDict(
-    "UpdateSlotResponseTypeDef",
+SlotValueElicitationSettingUnionTypeDef = Union[
+    SlotValueElicitationSettingTypeDef, SlotValueElicitationSettingOutputTypeDef
+]
+_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "slotName": str,
-        "description": str,
-        "slotTypeId": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeId": str,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
+
+class UpdateSlotRequestRequestTypeDef(
+    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/type_defs.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lexv2_models.type_defs import ActiveContextTypeDef
 
-    data: ActiveContextTypeDef = {...}
+    data: ActiveContextTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
     BotFilterNameType,
@@ -75,14 +75,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveContextTypeDef",
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
@@ -92,14 +93,15 @@
     "AssociatedTranscriptTypeDef",
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
     "CustomVocabularyItemTypeDef",
     "FailedCustomVocabularyItemTypeDef",
+    "ResponseMetadataTypeDef",
     "CustomVocabularyEntryIdTypeDef",
     "BotAliasHistoryEventTypeDef",
     "BotAliasSummaryTypeDef",
     "BotAliasTestExecutionTargetTypeDef",
     "BotExportSpecificationTypeDef",
     "BotFilterTypeDef",
     "DataPrivacyTypeDef",
@@ -115,101 +117,86 @@
     "BotRecommendationSummaryTypeDef",
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
     "BotVersionSummaryTypeDef",
     "BuildBotLocaleRequestRequestTypeDef",
-    "BuildBotLocaleResponseTypeDef",
     "BuiltInIntentSortByTypeDef",
     "BuiltInIntentSummaryTypeDef",
     "BuiltInSlotTypeSortByTypeDef",
     "BuiltInSlotTypeSummaryTypeDef",
     "ButtonTypeDef",
     "CloudWatchLogGroupLogDestinationTypeDef",
     "LambdaCodeHookTypeDef",
     "SubSlotTypeCompositionTypeDef",
     "ConditionTypeDef",
     "ConversationLevelIntentClassificationResultItemTypeDef",
     "ConversationLevelResultDetailTypeDef",
     "ConversationLevelSlotResolutionResultItemTypeDef",
     "ConversationLevelTestResultsFilterByTypeDef",
-    "ConversationLogsDataSourceFilterByTypeDef",
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
+    "TimestampTypeDef",
     "SentimentAnalysisSettingsTypeDef",
     "DialogCodeHookSettingsTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "SampleUtteranceTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
-    "CreateResourcePolicyResponseTypeDef",
     "PrincipalTypeDef",
-    "CreateResourcePolicyStatementResponseTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "CustomPayloadTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
-    "DateRangeFilterTypeDef",
+    "DateRangeFilterOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
-    "DeleteBotAliasResponseTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
-    "DeleteBotLocaleResponseTypeDef",
     "DeleteBotRequestRequestTypeDef",
-    "DeleteBotResponseTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
-    "DeleteBotVersionResponseTypeDef",
     "DeleteCustomVocabularyRequestRequestTypeDef",
-    "DeleteCustomVocabularyResponseTypeDef",
     "DeleteExportRequestRequestTypeDef",
-    "DeleteExportResponseTypeDef",
     "DeleteImportRequestRequestTypeDef",
-    "DeleteImportResponseTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
     "DeleteResourcePolicyStatementRequestRequestTypeDef",
-    "DeleteResourcePolicyStatementResponseTypeDef",
     "DeleteSlotRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteTestSetRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
     "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
     "EncryptionSettingTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeExportRequestRequestTypeDef",
     "DescribeImportRequestRequestTypeDef",
     "DescribeIntentRequestRequestTypeDef",
     "SlotPriorityTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSlotRequestRequestTypeDef",
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
     "TestSetStorageLocationTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
     "DialogActionTypeDef",
+    "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportFilterTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
     "IntentFilterTypeDef",
@@ -221,60 +208,78 @@
     "RecommendedIntentSummaryTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
     "PlainTextMessageTypeDef",
     "SSMLMessageTypeDef",
     "OverallTestResultItemTypeDef",
+    "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
     "TextInputSpecificationTypeDef",
     "RelativeAggregationDurationTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
     "SampleValueTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
     "SlotValueTypeDef",
     "SlotValueRegexFilterTypeDef",
     "StopBotRecommendationRequestRequestTypeDef",
-    "StopBotRecommendationResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSetIntentDiscrepancyItemTypeDef",
     "TestSetSlotDiscrepancyItemTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
     "TestSetImportInputLocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
-    "UpdateResourcePolicyResponseTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
-    "SearchAssociatedTranscriptsResponseTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
     "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
-    "ListCustomVocabularyItemsResponseTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
+    "BuildBotLocaleResponseTypeDef",
+    "CreateResourcePolicyResponseTypeDef",
+    "CreateResourcePolicyStatementResponseTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "DeleteBotAliasResponseTypeDef",
+    "DeleteBotLocaleResponseTypeDef",
+    "DeleteBotResponseTypeDef",
+    "DeleteBotVersionResponseTypeDef",
+    "DeleteCustomVocabularyResponseTypeDef",
+    "DeleteExportResponseTypeDef",
+    "DeleteImportResponseTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    "ListCustomVocabularyItemsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    "StopBotRecommendationResponseTypeDef",
+    "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "TestExecutionTargetTypeDef",
+    "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
     "BotLocaleImportSpecificationTypeDef",
     "CreateBotLocaleRequestRequestTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
     "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
@@ -293,37 +298,42 @@
     "CreateBotVersionResponseTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
     "ListBotVersionsResponseTypeDef",
     "ListBuiltInIntentsRequestRequestTypeDef",
     "ListBuiltInIntentsResponseTypeDef",
     "ListBuiltInSlotTypesRequestRequestTypeDef",
     "ListBuiltInSlotTypesResponseTypeDef",
+    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "TextLogDestinationTypeDef",
     "CodeHookSpecificationTypeDef",
+    "CompositeSlotTypeSettingOutputTypeDef",
     "CompositeSlotTypeSettingTypeDef",
     "ConversationLevelTestResultItemTypeDef",
     "TestExecutionResultFilterByTypeDef",
-    "ConversationLogsDataSourceTypeDef",
+    "ConversationLogsDataSourceOutputTypeDef",
+    "ConversationLogsDataSourceFilterByTypeDef",
+    "DateRangeFilterTypeDef",
     "IntentSummaryTypeDef",
     "CreateResourcePolicyStatementRequestRequestTypeDef",
-    "LexTranscriptFilterTypeDef",
+    "LexTranscriptFilterOutputTypeDef",
     "DescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
     "DescribeBotVersionResponseTypeDef",
     "UpdateBotRecommendationRequestRequestTypeDef",
     "DescribeTestSetResponseTypeDef",
     "TestSetSummaryTypeDef",
     "UpdateTestSetResponseTypeDef",
+    "DialogStateOutputTypeDef",
     "DialogStateTypeDef",
     "ExportResourceSpecificationTypeDef",
     "ListExportsRequestRequestTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "InputSessionStateSpecificationTypeDef",
@@ -334,126 +344,174 @@
     "ListSlotTypesResponseTypeDef",
     "ListSlotsRequestRequestTypeDef",
     "ListTestExecutionsRequestRequestTypeDef",
     "ListTestSetsRequestRequestTypeDef",
     "OverallTestResultsTypeDef",
     "UtteranceAggregationDurationTypeDef",
     "RuntimeHintDetailsTypeDef",
+    "SlotTypeValueOutputTypeDef",
     "SlotTypeValueTypeDef",
+    "SlotDefaultValueSpecificationOutputTypeDef",
     "SlotDefaultValueSpecificationTypeDef",
     "SlotResolutionTestResultItemTypeDef",
+    "SlotValueOverrideOutputTypeDef",
     "SlotValueOverrideTypeDef",
     "SlotValueSelectionSettingTypeDef",
     "TestSetDiscrepancyErrorsTypeDef",
     "TestSetDiscrepancyReportResourceTargetTypeDef",
+    "TestSetImportResourceSpecificationOutputTypeDef",
     "TestSetImportResourceSpecificationTypeDef",
     "UserTurnOutputSpecificationTypeDef",
     "UtteranceInputSpecificationTypeDef",
     "PromptAttemptSpecificationTypeDef",
     "AudioLogSettingTypeDef",
     "DescribeTestExecutionResponseTypeDef",
     "StartTestExecutionRequestRequestTypeDef",
     "StartTestExecutionResponseTypeDef",
     "TestExecutionSummaryTypeDef",
     "BotRecommendationResultsTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
     "TextLogSettingTypeDef",
     "BotAliasLocaleSettingsTypeDef",
+    "CompositeSlotTypeSettingUnionTypeDef",
     "ConversationLevelTestResultsTypeDef",
     "ListTestExecutionResultItemsRequestRequestTypeDef",
-    "TestSetGenerationDataSourceTypeDef",
+    "TestSetGenerationDataSourceOutputTypeDef",
+    "ConversationLogsDataSourceTypeDef",
+    "LexTranscriptFilterTypeDef",
     "ListIntentsResponseTypeDef",
-    "TranscriptFilterTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "ListTestSetsResponseTypeDef",
     "CreateExportRequestRequestTypeDef",
     "CreateExportResponseTypeDef",
     "DescribeExportResponseTypeDef",
     "ExportSummaryTypeDef",
     "UpdateExportResponseTypeDef",
     "ExternalSourceSettingTypeDef",
     "IntentClassificationTestResultsTypeDef",
     "ListAggregatedUtterancesRequestRequestTypeDef",
     "ListAggregatedUtterancesResponseTypeDef",
+    "SlotTypeValueUnionTypeDef",
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
+    "ImportResourceSpecificationOutputTypeDef",
     "ImportResourceSpecificationTypeDef",
     "UserTurnInputSpecificationTypeDef",
     "ListTestExecutionsResponseTypeDef",
+    "MessageGroupOutputTypeDef",
     "MessageGroupTypeDef",
+    "ConversationLogSettingsOutputTypeDef",
     "ConversationLogSettingsTypeDef",
     "DescribeTestSetGenerationResponseTypeDef",
-    "StartTestSetGenerationRequestRequestTypeDef",
     "StartTestSetGenerationResponseTypeDef",
-    "S3BucketTranscriptSourceTypeDef",
+    "TestSetGenerationDataSourceTypeDef",
+    "TranscriptFilterTypeDef",
+    "S3BucketTranscriptSourceOutputTypeDef",
     "ListExportsResponseTypeDef",
-    "CreateSlotTypeRequestRequestTypeDef",
     "CreateSlotTypeResponseTypeDef",
     "DescribeSlotTypeResponseTypeDef",
-    "UpdateSlotTypeRequestRequestTypeDef",
     "UpdateSlotTypeResponseTypeDef",
+    "CreateSlotTypeRequestRequestTypeDef",
+    "UpdateSlotTypeRequestRequestTypeDef",
     "IntentLevelSlotResolutionTestResultsTypeDef",
     "DescribeImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
+    "ImportResourceSpecificationUnionTypeDef",
+    "StartImportRequestRequestTypeDef",
     "UserTurnResultTypeDef",
     "UserTurnSpecificationTypeDef",
+    "FulfillmentStartResponseSpecificationOutputTypeDef",
+    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
+    "PromptSpecificationOutputTypeDef",
+    "ResponseSpecificationOutputTypeDef",
+    "StillWaitingResponseSpecificationOutputTypeDef",
     "FulfillmentStartResponseSpecificationTypeDef",
     "FulfillmentUpdateResponseSpecificationTypeDef",
     "PromptSpecificationTypeDef",
     "ResponseSpecificationTypeDef",
     "StillWaitingResponseSpecificationTypeDef",
-    "CreateBotAliasRequestRequestTypeDef",
     "CreateBotAliasResponseTypeDef",
     "DescribeBotAliasResponseTypeDef",
-    "UpdateBotAliasRequestRequestTypeDef",
     "UpdateBotAliasResponseTypeDef",
-    "TranscriptSourceSettingTypeDef",
+    "ConversationLogSettingsUnionTypeDef",
+    "CreateBotAliasRequestRequestTypeDef",
+    "UpdateBotAliasRequestRequestTypeDef",
+    "StartTestSetGenerationRequestRequestTypeDef",
+    "TestSetGenerationDataSourceUnionTypeDef",
+    "S3BucketTranscriptSourceTypeDef",
+    "TranscriptSourceSettingOutputTypeDef",
     "TestSetTurnResultTypeDef",
     "TurnSpecificationTypeDef",
-    "FulfillmentUpdatesSpecificationTypeDef",
+    "FulfillmentUpdatesSpecificationOutputTypeDef",
     "SlotSummaryTypeDef",
+    "ConditionalBranchOutputTypeDef",
+    "DefaultConditionalBranchOutputTypeDef",
+    "WaitAndContinueSpecificationOutputTypeDef",
+    "FulfillmentUpdatesSpecificationTypeDef",
     "ConditionalBranchTypeDef",
     "DefaultConditionalBranchTypeDef",
     "WaitAndContinueSpecificationTypeDef",
+    "TranscriptSourceSettingTypeDef",
     "DescribeBotRecommendationResponseTypeDef",
-    "StartBotRecommendationRequestRequestTypeDef",
     "StartBotRecommendationResponseTypeDef",
     "UpdateBotRecommendationResponseTypeDef",
     "UtteranceLevelTestResultItemTypeDef",
     "TestSetTurnRecordTypeDef",
     "ListSlotsResponseTypeDef",
+    "ConditionalSpecificationOutputTypeDef",
+    "SubSlotValueElicitationSettingOutputTypeDef",
     "ConditionalSpecificationTypeDef",
     "SubSlotValueElicitationSettingTypeDef",
+    "StartBotRecommendationRequestRequestTypeDef",
+    "TranscriptSourceSettingUnionTypeDef",
     "UtteranceLevelTestResultsTypeDef",
     "ListTestSetRecordsResponseTypeDef",
+    "IntentClosingSettingOutputTypeDef",
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    "SpecificationsOutputTypeDef",
     "IntentClosingSettingTypeDef",
     "PostDialogCodeHookInvocationSpecificationTypeDef",
     "PostFulfillmentStatusSpecificationTypeDef",
     "SpecificationsTypeDef",
     "TestExecutionResultItemsTypeDef",
+    "DialogCodeHookInvocationSettingOutputTypeDef",
+    "FulfillmentCodeHookSettingsOutputTypeDef",
+    "SubSlotSettingOutputTypeDef",
+    "IntentClosingSettingUnionTypeDef",
     "DialogCodeHookInvocationSettingTypeDef",
     "FulfillmentCodeHookSettingsTypeDef",
     "SubSlotSettingTypeDef",
     "ListTestExecutionResultItemsResponseTypeDef",
+    "InitialResponseSettingOutputTypeDef",
+    "IntentConfirmationSettingOutputTypeDef",
+    "SlotCaptureSettingOutputTypeDef",
     "InitialResponseSettingTypeDef",
     "IntentConfirmationSettingTypeDef",
     "SlotCaptureSettingTypeDef",
-    "CreateIntentRequestRequestTypeDef",
+    "FulfillmentCodeHookSettingsUnionTypeDef",
+    "SubSlotSettingUnionTypeDef",
     "CreateIntentResponseTypeDef",
     "DescribeIntentResponseTypeDef",
-    "UpdateIntentRequestRequestTypeDef",
     "UpdateIntentResponseTypeDef",
+    "SlotValueElicitationSettingOutputTypeDef",
+    "InitialResponseSettingUnionTypeDef",
+    "CreateIntentRequestRequestTypeDef",
+    "IntentConfirmationSettingUnionTypeDef",
+    "UpdateIntentRequestRequestTypeDef",
     "SlotValueElicitationSettingTypeDef",
-    "CreateSlotRequestRequestTypeDef",
     "CreateSlotResponseTypeDef",
     "DescribeSlotResponseTypeDef",
-    "UpdateSlotRequestRequestTypeDef",
     "UpdateSlotResponseTypeDef",
+    "CreateSlotRequestRequestTypeDef",
+    "SlotValueElicitationSettingUnionTypeDef",
+    "UpdateSlotRequestRequestTypeDef",
 )
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
     },
@@ -565,19 +623,21 @@
     "_OptionalS3BucketLogDestinationTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class S3BucketLogDestinationTypeDef(
     _RequiredS3BucketLogDestinationTypeDef, _OptionalS3BucketLogDestinationTypeDef
 ):
     pass
 
+
 _RequiredNewCustomVocabularyItemTypeDef = TypedDict(
     "_RequiredNewCustomVocabularyItemTypeDef",
     {
         "phrase": str,
     },
 )
 _OptionalNewCustomVocabularyItemTypeDef = TypedDict(
@@ -585,19 +645,21 @@
     {
         "weight": int,
         "displayAs": str,
     },
     total=False,
 )
 
+
 class NewCustomVocabularyItemTypeDef(
     _RequiredNewCustomVocabularyItemTypeDef, _OptionalNewCustomVocabularyItemTypeDef
 ):
     pass
 
+
 _RequiredCustomVocabularyItemTypeDef = TypedDict(
     "_RequiredCustomVocabularyItemTypeDef",
     {
         "itemId": str,
         "phrase": str,
     },
 )
@@ -606,29 +668,42 @@
     {
         "weight": int,
         "displayAs": str,
     },
     total=False,
 )
 
+
 class CustomVocabularyItemTypeDef(
     _RequiredCustomVocabularyItemTypeDef, _OptionalCustomVocabularyItemTypeDef
 ):
     pass
 
+
 FailedCustomVocabularyItemTypeDef = TypedDict(
     "FailedCustomVocabularyItemTypeDef",
     {
         "itemId": str,
         "errorMessage": str,
         "errorCode": ErrorCodeType,
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
 CustomVocabularyEntryIdTypeDef = TypedDict(
     "CustomVocabularyEntryIdTypeDef",
     {
         "itemId": str,
     },
 )
 
@@ -725,17 +800,19 @@
     "_OptionalVoiceSettingsTypeDef",
     {
         "engine": VoiceEngineType,
     },
     total=False,
 )
 
+
 class VoiceSettingsTypeDef(_RequiredVoiceSettingsTypeDef, _OptionalVoiceSettingsTypeDef):
     pass
 
+
 BotLocaleSortByTypeDef = TypedDict(
     "BotLocaleSortByTypeDef",
     {
         "attribute": Literal["BotLocaleName"],
         "order": SortOrderType,
     },
 )
@@ -792,19 +869,21 @@
     {
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+
 class BotRecommendationSummaryTypeDef(
     _RequiredBotRecommendationSummaryTypeDef, _OptionalBotRecommendationSummaryTypeDef
 ):
     pass
 
+
 BotSortByTypeDef = TypedDict(
     "BotSortByTypeDef",
     {
         "attribute": Literal["BotName"],
         "order": SortOrderType,
     },
 )
@@ -855,26 +934,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-BuildBotLocaleResponseTypeDef = TypedDict(
-    "BuildBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "lastBuildSubmittedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BuiltInIntentSortByTypeDef = TypedDict(
     "BuiltInIntentSortByTypeDef",
     {
         "attribute": Literal["IntentSignature"],
         "order": SortOrderType,
     },
 )
@@ -962,19 +1029,21 @@
     "_OptionalConversationLevelResultDetailTypeDef",
     {
         "speechTranscriptionResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
+
 class ConversationLevelResultDetailTypeDef(
     _RequiredConversationLevelResultDetailTypeDef, _OptionalConversationLevelResultDetailTypeDef
 ):
     pass
 
+
 ConversationLevelSlotResolutionResultItemTypeDef = TypedDict(
     "ConversationLevelSlotResolutionResultItemTypeDef",
     {
         "intentName": str,
         "slotName": str,
         "matchResult": TestResultMatchStatusType,
     },
@@ -984,23 +1053,24 @@
     "ConversationLevelTestResultsFilterByTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-ConversationLogsDataSourceFilterByTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByTypeDef",
+ConversationLogsDataSourceFilterByOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
         "inputMode": ConversationLogsInputModeFilterType,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 SentimentAnalysisSettingsTypeDef = TypedDict(
     "SentimentAnalysisSettingsTypeDef",
     {
         "detectSentiment": bool,
     },
 )
 
@@ -1029,19 +1099,21 @@
     {
         "queryFilterStringEnabled": bool,
         "queryFilterString": str,
     },
     total=False,
 )
 
+
 class KendraConfigurationTypeDef(
     _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
 ):
     pass
 
+
 OutputContextTypeDef = TypedDict(
     "OutputContextTypeDef",
     {
         "name": str,
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
@@ -1058,41 +1130,23 @@
     "CreateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
 
-CreateResourcePolicyResponseTypeDef = TypedDict(
-    "CreateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "service": str,
         "arn": str,
     },
     total=False,
 )
 
-CreateResourcePolicyStatementResponseTypeDef = TypedDict(
-    "CreateResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MultipleValuesSettingTypeDef = TypedDict(
     "MultipleValuesSettingTypeDef",
     {
         "allowMultipleValues": bool,
     },
     total=False,
 )
@@ -1100,23 +1154,14 @@
 ObfuscationSettingTypeDef = TypedDict(
     "ObfuscationSettingTypeDef",
     {
         "obfuscationSettingType": ObfuscationSettingTypeType,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "importId": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomPayloadTypeDef = TypedDict(
     "CustomPayloadTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1134,16 +1179,16 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DateRangeFilterTypeDef = TypedDict(
-    "DateRangeFilterTypeDef",
+DateRangeFilterOutputTypeDef = TypedDict(
+    "DateRangeFilterOutputTypeDef",
     {
         "startDateTime": datetime,
         "endDateTime": datetime,
     },
 )
 
 _RequiredDeleteBotAliasRequestRequestTypeDef = TypedDict(
@@ -1157,76 +1202,50 @@
     "_OptionalDeleteBotAliasRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
+
 class DeleteBotAliasRequestRequestTypeDef(
     _RequiredDeleteBotAliasRequestRequestTypeDef, _OptionalDeleteBotAliasRequestRequestTypeDef
 ):
     pass
 
-DeleteBotAliasResponseTypeDef = TypedDict(
-    "DeleteBotAliasResponseTypeDef",
-    {
-        "botAliasId": str,
-        "botId": str,
-        "botAliasStatus": BotAliasStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteBotLocaleRequestRequestTypeDef = TypedDict(
     "DeleteBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteBotLocaleResponseTypeDef = TypedDict(
-    "DeleteBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalDeleteBotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBotRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
+
 class DeleteBotRequestRequestTypeDef(
     _RequiredDeleteBotRequestRequestTypeDef, _OptionalDeleteBotRequestRequestTypeDef
 ):
     pass
 
-DeleteBotResponseTypeDef = TypedDict(
-    "DeleteBotResponseTypeDef",
-    {
-        "botId": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotVersionRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
@@ -1235,81 +1254,44 @@
     "_OptionalDeleteBotVersionRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
+
 class DeleteBotVersionRequestRequestTypeDef(
     _RequiredDeleteBotVersionRequestRequestTypeDef, _OptionalDeleteBotVersionRequestRequestTypeDef
 ):
     pass
 
-DeleteBotVersionResponseTypeDef = TypedDict(
-    "DeleteBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteCustomVocabularyRequestRequestTypeDef = TypedDict(
     "DeleteCustomVocabularyRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteCustomVocabularyResponseTypeDef = TypedDict(
-    "DeleteCustomVocabularyResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteExportRequestRequestTypeDef = TypedDict(
     "DeleteExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-DeleteExportResponseTypeDef = TypedDict(
-    "DeleteExportResponseTypeDef",
-    {
-        "exportId": str,
-        "exportStatus": ExportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImportRequestRequestTypeDef = TypedDict(
     "DeleteImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-DeleteImportResponseTypeDef = TypedDict(
-    "DeleteImportResponseTypeDef",
-    {
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIntentRequestRequestTypeDef = TypedDict(
     "DeleteIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -1326,28 +1308,21 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "expectedRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourcePolicyStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "statementId": str,
     },
@@ -1356,28 +1331,21 @@
     "_OptionalDeleteResourcePolicyStatementRequestRequestTypeDef",
     {
         "expectedRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteResourcePolicyStatementRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
-DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteSlotRequestRequestTypeDef = TypedDict(
     "DeleteSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
@@ -1399,19 +1367,21 @@
     "_OptionalDeleteSlotTypeRequestRequestTypeDef",
     {
         "skipResourceInUseCheck": bool,
     },
     total=False,
 )
 
+
 class DeleteSlotTypeRequestRequestTypeDef(
     _RequiredDeleteSlotTypeRequestRequestTypeDef, _OptionalDeleteSlotTypeRequestRequestTypeDef
 ):
     pass
 
+
 DeleteTestSetRequestRequestTypeDef = TypedDict(
     "DeleteTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
     },
 )
 
@@ -1426,19 +1396,21 @@
     {
         "localeId": str,
         "sessionId": str,
     },
     total=False,
 )
 
+
 class DeleteUtterancesRequestRequestTypeDef(
     _RequiredDeleteUtterancesRequestRequestTypeDef, _OptionalDeleteUtterancesRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1509,27 +1481,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExportRequestRequestTypeDef = TypedDict(
     "DescribeExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
@@ -1561,24 +1520,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSlotRequestRequestTypeDef = TypedDict(
     "DescribeSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -1628,19 +1577,21 @@
     "_OptionalTestSetStorageLocationTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class TestSetStorageLocationTypeDef(
     _RequiredTestSetStorageLocationTypeDef, _OptionalTestSetStorageLocationTypeDef
 ):
     pass
 
+
 DescribeTestSetRequestRequestTypeDef = TypedDict(
     "DescribeTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
     },
 )
 
@@ -1655,17 +1606,28 @@
     {
         "slotToElicit": str,
         "suppressNextMessage": bool,
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+
+IntentOverrideOutputTypeDef = TypedDict(
+    "IntentOverrideOutputTypeDef",
+    {
+        "name": str,
+        "slots": Dict[str, "SlotValueOverrideOutputTypeDef"],
+    },
+    total=False,
+)
+
 IntentOverrideTypeDef = TypedDict(
     "IntentOverrideTypeDef",
     {
         "name": str,
         "slots": Mapping[str, "SlotValueOverrideTypeDef"],
     },
     total=False,
@@ -1681,26 +1643,21 @@
     "_OptionalElicitationCodeHookInvocationSettingTypeDef",
     {
         "invocationLabel": str,
     },
     total=False,
 )
 
+
 class ElicitationCodeHookInvocationSettingTypeDef(
     _RequiredElicitationCodeHookInvocationSettingTypeDef,
     _OptionalElicitationCodeHookInvocationSettingTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ExportFilterTypeDef = TypedDict(
     "ExportFilterTypeDef",
     {
         "name": Literal["ExportResourceType"],
         "values": Sequence[str],
         "operator": ExportFilterOperatorType,
@@ -1725,23 +1682,14 @@
 GetTestExecutionArtifactsUrlRequestRequestTypeDef = TypedDict(
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     {
         "testExecutionId": str,
     },
 )
 
-GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
-    {
-        "testExecutionId": str,
-        "downloadArtifactsUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGrammarSlotTypeSourceTypeDef = TypedDict(
     "_RequiredGrammarSlotTypeSourceTypeDef",
     {
         "s3BucketName": str,
         "s3ObjectKey": str,
     },
 )
@@ -1749,19 +1697,21 @@
     "_OptionalGrammarSlotTypeSourceTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class GrammarSlotTypeSourceTypeDef(
     _RequiredGrammarSlotTypeSourceTypeDef, _OptionalGrammarSlotTypeSourceTypeDef
 ):
     pass
 
+
 ImportFilterTypeDef = TypedDict(
     "ImportFilterTypeDef",
     {
         "name": Literal["ImportResourceType"],
         "values": Sequence[str],
         "operator": ImportFilterOperatorType,
     },
@@ -1809,20 +1759,22 @@
     "_OptionalIntentClassificationTestResultItemCountsTypeDef",
     {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
     },
     total=False,
 )
 
+
 class IntentClassificationTestResultItemCountsTypeDef(
     _RequiredIntentClassificationTestResultItemCountsTypeDef,
     _OptionalIntentClassificationTestResultItemCountsTypeDef,
 ):
     pass
 
+
 IntentFilterTypeDef = TypedDict(
     "IntentFilterTypeDef",
     {
         "name": Literal["IntentName"],
         "values": Sequence[str],
         "operator": IntentFilterOperatorType,
     },
@@ -1847,19 +1799,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBotAliasesRequestRequestTypeDef(
     _RequiredListBotAliasesRequestRequestTypeDef, _OptionalListBotAliasesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListBotRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotRecommendationsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -1869,20 +1823,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBotRecommendationsRequestRequestTypeDef(
     _RequiredListBotRecommendationsRequestRequestTypeDef,
     _OptionalListBotRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListCustomVocabularyItemsRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomVocabularyItemsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -1892,20 +1848,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListCustomVocabularyItemsRequestRequestTypeDef(
     _RequiredListCustomVocabularyItemsRequestRequestTypeDef,
     _OptionalListCustomVocabularyItemsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListRecommendedIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendedIntentsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -1916,20 +1874,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListRecommendedIntentsRequestRequestTypeDef(
     _RequiredListRecommendedIntentsRequestRequestTypeDef,
     _OptionalListRecommendedIntentsRequestRequestTypeDef,
 ):
     pass
 
+
 RecommendedIntentSummaryTypeDef = TypedDict(
     "RecommendedIntentSummaryTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "sampleUtterancesCount": int,
     },
@@ -1986,22 +1946,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
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
 TestExecutionSortByTypeDef = TypedDict(
     "TestExecutionSortByTypeDef",
     {
         "attribute": TestExecutionSortAttributeType,
         "order": SortOrderType,
     },
 )
@@ -2017,20 +1969,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTestSetRecordsRequestRequestTypeDef(
     _RequiredListTestSetRecordsRequestRequestTypeDef,
     _OptionalListTestSetRecordsRequestRequestTypeDef,
 ):
     pass
 
+
 TestSetSortByTypeDef = TypedDict(
     "TestSetSortByTypeDef",
     {
         "attribute": TestSetSortAttributeType,
         "order": SortOrderType,
     },
 )
@@ -2061,23 +2015,33 @@
     "_OptionalOverallTestResultItemTypeDef",
     {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
     },
     total=False,
 )
 
+
 class OverallTestResultItemTypeDef(
     _RequiredOverallTestResultItemTypeDef, _OptionalOverallTestResultItemTypeDef
 ):
     pass
 
+
+PathFormatOutputTypeDef = TypedDict(
+    "PathFormatOutputTypeDef",
+    {
+        "objectPrefixes": List[str],
+    },
+    total=False,
+)
+
 PathFormatTypeDef = TypedDict(
     "PathFormatTypeDef",
     {
-        "objectPrefixes": List[str],
+        "objectPrefixes": Sequence[str],
     },
     total=False,
 )
 
 TextInputSpecificationTypeDef = TypedDict(
     "TextInputSpecificationTypeDef",
     {
@@ -2089,25 +2053,14 @@
     "RelativeAggregationDurationTypeDef",
     {
         "timeDimension": TimeDimensionType,
         "timeValue": int,
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
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -2136,20 +2089,22 @@
     "_OptionalSlotResolutionTestResultItemCountsTypeDef",
     {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
     },
     total=False,
 )
 
+
 class SlotResolutionTestResultItemCountsTypeDef(
     _RequiredSlotResolutionTestResultItemCountsTypeDef,
     _OptionalSlotResolutionTestResultItemCountsTypeDef,
 ):
     pass
 
+
 SlotValueTypeDef = TypedDict(
     "SlotValueTypeDef",
     {
         "interpretedValue": str,
     },
     total=False,
 )
@@ -2167,26 +2122,14 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
     },
 )
 
-StopBotRecommendationResponseTypeDef = TypedDict(
-    "StopBotRecommendationResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationStatus": BotRecommendationStatusType,
-        "botRecommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2243,19 +2186,21 @@
     "_OptionalUpdateExportRequestRequestTypeDef",
     {
         "filePassword": str,
     },
     total=False,
 )
 
+
 class UpdateExportRequestRequestTypeDef(
     _RequiredUpdateExportRequestRequestTypeDef, _OptionalUpdateExportRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
@@ -2263,28 +2208,21 @@
     "_OptionalUpdateResourcePolicyRequestRequestTypeDef",
     {
         "expectedRevisionId": str,
     },
     total=False,
 )
 
+
 class UpdateResourcePolicyRequestRequestTypeDef(
     _RequiredUpdateResourcePolicyRequestRequestTypeDef,
     _OptionalUpdateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-UpdateResourcePolicyResponseTypeDef = TypedDict(
-    "UpdateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateTestSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
     },
@@ -2293,38 +2231,42 @@
     "_OptionalUpdateTestSetRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateTestSetRequestRequestTypeDef(
     _RequiredUpdateTestSetRequestRequestTypeDef, _OptionalUpdateTestSetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUserTurnIntentOutputTypeDef = TypedDict(
     "_RequiredUserTurnIntentOutputTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUserTurnIntentOutputTypeDef = TypedDict(
     "_OptionalUserTurnIntentOutputTypeDef",
     {
         "slots": Dict[str, "UserTurnSlotOutputTypeDef"],
     },
     total=False,
 )
 
+
 class UserTurnIntentOutputTypeDef(
     _RequiredUserTurnIntentOutputTypeDef, _OptionalUserTurnIntentOutputTypeDef
 ):
     pass
 
+
 UserTurnSlotOutputTypeDef = TypedDict(
     "UserTurnSlotOutputTypeDef",
     {
         "value": str,
         "values": List[Dict[str, Any]],
         "subSlots": Dict[str, Dict[str, Any]],
     },
@@ -2351,17 +2293,19 @@
         "errorDetails": ExecutionErrorDetailsTypeDef,
         "actualElicitedSlot": str,
         "actualIntent": str,
     },
     total=False,
 )
 
+
 class AgentTurnResultTypeDef(_RequiredAgentTurnResultTypeDef, _OptionalAgentTurnResultTypeDef):
     pass
 
+
 _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAssociatedTranscriptsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -2374,33 +2318,21 @@
         "searchOrder": SearchOrderType,
         "maxResults": int,
         "nextIndex": int,
     },
     total=False,
 )
 
+
 class SearchAssociatedTranscriptsRequestRequestTypeDef(
     _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef,
     _OptionalSearchAssociatedTranscriptsRequestRequestTypeDef,
 ):
     pass
 
-SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
-    "SearchAssociatedTranscriptsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationId": str,
-        "nextIndex": int,
-        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
-        "totalResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredAudioAndDTMFInputSpecificationTypeDef = TypedDict(
     "_RequiredAudioAndDTMFInputSpecificationTypeDef",
     {
         "startTimeoutMs": int,
     },
 )
@@ -2409,19 +2341,21 @@
     {
         "audioSpecification": AudioSpecificationTypeDef,
         "dtmfSpecification": DTMFSpecificationTypeDef,
     },
     total=False,
 )
 
+
 class AudioAndDTMFInputSpecificationTypeDef(
     _RequiredAudioAndDTMFInputSpecificationTypeDef, _OptionalAudioAndDTMFInputSpecificationTypeDef
 ):
     pass
 
+
 AudioLogDestinationTypeDef = TypedDict(
     "AudioLogDestinationTypeDef",
     {
         "s3Bucket": S3BucketLogDestinationTypeDef,
     },
 )
 
@@ -2441,59 +2375,267 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[CustomVocabularyItemTypeDef],
     },
 )
 
-ListCustomVocabularyItemsResponseTypeDef = TypedDict(
-    "ListCustomVocabularyItemsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyItems": List[CustomVocabularyItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchCreateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BuildBotLocaleResponseTypeDef = TypedDict(
+    "BuildBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "lastBuildSubmittedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyResponseTypeDef = TypedDict(
+    "CreateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyStatementResponseTypeDef = TypedDict(
+    "CreateResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "importId": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotAliasResponseTypeDef = TypedDict(
+    "DeleteBotAliasResponseTypeDef",
+    {
+        "botAliasId": str,
+        "botId": str,
+        "botAliasStatus": BotAliasStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotLocaleResponseTypeDef = TypedDict(
+    "DeleteBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotResponseTypeDef = TypedDict(
+    "DeleteBotResponseTypeDef",
+    {
+        "botId": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotVersionResponseTypeDef = TypedDict(
+    "DeleteBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomVocabularyResponseTypeDef = TypedDict(
+    "DeleteCustomVocabularyResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteExportResponseTypeDef = TypedDict(
+    "DeleteExportResponseTypeDef",
+    {
+        "exportId": str,
+        "exportStatus": ExportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImportResponseTypeDef = TypedDict(
+    "DeleteImportResponseTypeDef",
+    {
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "policy": str,
+        "revisionId": str,
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
+GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    {
+        "testExecutionId": str,
+        "downloadArtifactsUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVocabularyItemsResponseTypeDef = TypedDict(
+    "ListCustomVocabularyItemsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyItems": List[CustomVocabularyItemTypeDef],
+        "nextToken": str,
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
+SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationId": str,
+        "nextIndex": int,
+        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
+        "totalResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopBotRecommendationResponseTypeDef = TypedDict(
+    "StopBotRecommendationResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationStatus": BotRecommendationStatusType,
+        "botRecommendationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateResourcePolicyResponseTypeDef = TypedDict(
+    "UpdateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemRequestRequestTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     {
         "botId": str,
@@ -2505,49 +2647,76 @@
 
 ListBotAliasesResponseTypeDef = TypedDict(
     "ListBotAliasesResponseTypeDef",
     {
         "botAliasSummaries": List[BotAliasSummaryTypeDef],
         "nextToken": str,
         "botId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionTargetTypeDef = TypedDict(
     "TestExecutionTargetTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetTypeDef,
     },
     total=False,
 )
 
+_RequiredBotImportSpecificationOutputTypeDef = TypedDict(
+    "_RequiredBotImportSpecificationOutputTypeDef",
+    {
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+    },
+)
+_OptionalBotImportSpecificationOutputTypeDef = TypedDict(
+    "_OptionalBotImportSpecificationOutputTypeDef",
+    {
+        "idleSessionTTLInSeconds": int,
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class BotImportSpecificationOutputTypeDef(
+    _RequiredBotImportSpecificationOutputTypeDef, _OptionalBotImportSpecificationOutputTypeDef
+):
+    pass
+
+
 _RequiredBotImportSpecificationTypeDef = TypedDict(
     "_RequiredBotImportSpecificationTypeDef",
     {
         "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
     },
 )
 _OptionalBotImportSpecificationTypeDef = TypedDict(
     "_OptionalBotImportSpecificationTypeDef",
     {
         "idleSessionTTLInSeconds": int,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
     pass
 
+
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2557,19 +2726,21 @@
     {
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class BotLocaleImportSpecificationTypeDef(
     _RequiredBotLocaleImportSpecificationTypeDef, _OptionalBotLocaleImportSpecificationTypeDef
 ):
     pass
 
+
 _RequiredCreateBotLocaleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "nluIntentConfidenceThreshold": float,
@@ -2580,32 +2751,34 @@
     {
         "description": str,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateBotLocaleRequestRequestTypeDef(
     _RequiredCreateBotLocaleRequestRequestTypeDef, _OptionalCreateBotLocaleRequestRequestTypeDef
 ):
     pass
 
+
 CreateBotLocaleResponseTypeDef = TypedDict(
     "CreateBotLocaleResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeName": str,
         "localeId": str,
         "description": str,
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotLocaleResponseTypeDef = TypedDict(
     "DescribeBotLocaleResponseTypeDef",
     {
         "botId": str,
@@ -2620,15 +2793,15 @@
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
         "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBotLocaleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
@@ -2642,19 +2815,21 @@
     {
         "description": str,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBotLocaleRequestRequestTypeDef(
     _RequiredUpdateBotLocaleRequestRequestTypeDef, _OptionalUpdateBotLocaleRequestRequestTypeDef
 ):
     pass
 
+
 UpdateBotLocaleResponseTypeDef = TypedDict(
     "UpdateBotLocaleResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "localeName": str,
@@ -2662,15 +2837,15 @@
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBotLocalesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotLocalesRequestRequestTypeDef",
     {
         "botId": str,
@@ -2684,27 +2859,29 @@
         "filters": Sequence[BotLocaleFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBotLocalesRequestRequestTypeDef(
     _RequiredListBotLocalesRequestRequestTypeDef, _OptionalListBotLocalesRequestRequestTypeDef
 ):
     pass
 
+
 ListBotLocalesResponseTypeDef = TypedDict(
     "ListBotLocalesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "botName": str,
@@ -2721,19 +2898,21 @@
         "testBotAliasTags": Mapping[str, str],
         "botType": BotTypeType,
         "botMembers": Sequence[BotMemberTypeDef],
     },
     total=False,
 )
 
+
 class CreateBotRequestRequestTypeDef(
     _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
 ):
     pass
 
+
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
@@ -2741,15 +2920,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "botTags": Dict[str, str],
         "testBotAliasTags": Dict[str, str],
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotResponseTypeDef = TypedDict(
     "DescribeBotResponseTypeDef",
     {
         "botId": str,
@@ -2760,15 +2939,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "botId": str,
@@ -2784,34 +2963,36 @@
         "description": str,
         "botType": BotTypeType,
         "botMembers": Sequence[BotMemberTypeDef],
     },
     total=False,
 )
 
+
 class UpdateBotRequestRequestTypeDef(
     _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
 ):
     pass
 
+
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BotRecommendationResultStatisticsTypeDef = TypedDict(
     "BotRecommendationResultStatisticsTypeDef",
     {
         "intents": IntentStatisticsTypeDef,
@@ -2824,15 +3005,15 @@
     "ListBotRecommendationsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationSummaries": List[BotRecommendationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsRequestRequestTypeDef = TypedDict(
     "ListBotsRequestRequestTypeDef",
     {
         "sortBy": BotSortByTypeDef,
@@ -2844,15 +3025,15 @@
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "botSummaries": List[BotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotVersionRequestRequestTypeDef",
     {
         "botId": str,
@@ -2863,29 +3044,31 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
+
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "botId": str,
         "description": str,
         "botVersion": str,
         "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsTypeDef],
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotVersionsRequestRequestTypeDef",
     {
         "botId": str,
@@ -2897,26 +3080,28 @@
         "sortBy": BotVersionSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBotVersionsRequestRequestTypeDef(
     _RequiredListBotVersionsRequestRequestTypeDef, _OptionalListBotVersionsRequestRequestTypeDef
 ):
     pass
 
+
 ListBotVersionsResponseTypeDef = TypedDict(
     "ListBotVersionsResponseTypeDef",
     {
         "botId": str,
         "botVersionSummaries": List[BotVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInIntentsRequestRequestTypeDef",
     {
         "localeId": str,
@@ -2928,27 +3113,29 @@
         "sortBy": BuiltInIntentSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBuiltInIntentsRequestRequestTypeDef(
     _RequiredListBuiltInIntentsRequestRequestTypeDef,
     _OptionalListBuiltInIntentsRequestRequestTypeDef,
 ):
     pass
 
+
 ListBuiltInIntentsResponseTypeDef = TypedDict(
     "ListBuiltInIntentsResponseTypeDef",
     {
         "builtInIntentSummaries": List[BuiltInIntentSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInSlotTypesRequestRequestTypeDef",
     {
         "localeId": str,
@@ -2960,29 +3147,54 @@
         "sortBy": BuiltInSlotTypeSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBuiltInSlotTypesRequestRequestTypeDef(
     _RequiredListBuiltInSlotTypesRequestRequestTypeDef,
     _OptionalListBuiltInSlotTypesRequestRequestTypeDef,
 ):
     pass
 
+
 ListBuiltInSlotTypesResponseTypeDef = TypedDict(
     "ListBuiltInSlotTypesResponseTypeDef",
     {
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredImageResponseCardOutputTypeDef = TypedDict(
+    "_RequiredImageResponseCardOutputTypeDef",
+    {
+        "title": str,
     },
 )
+_OptionalImageResponseCardOutputTypeDef = TypedDict(
+    "_OptionalImageResponseCardOutputTypeDef",
+    {
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+
+class ImageResponseCardOutputTypeDef(
+    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
+):
+    pass
+
 
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
@@ -2992,33 +3204,43 @@
         "subtitle": str,
         "imageUrl": str,
         "buttons": Sequence[ButtonTypeDef],
     },
     total=False,
 )
 
+
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
+
 TextLogDestinationTypeDef = TypedDict(
     "TextLogDestinationTypeDef",
     {
         "cloudWatch": CloudWatchLogGroupLogDestinationTypeDef,
     },
 )
 
 CodeHookSpecificationTypeDef = TypedDict(
     "CodeHookSpecificationTypeDef",
     {
         "lambdaCodeHook": LambdaCodeHookTypeDef,
     },
 )
 
+CompositeSlotTypeSettingOutputTypeDef = TypedDict(
+    "CompositeSlotTypeSettingOutputTypeDef",
+    {
+        "subSlots": List[SubSlotTypeCompositionTypeDef],
+    },
+    total=False,
+)
+
 CompositeSlotTypeSettingTypeDef = TypedDict(
     "CompositeSlotTypeSettingTypeDef",
     {
         "subSlots": Sequence[SubSlotTypeCompositionTypeDef],
     },
     total=False,
 )
@@ -3036,45 +3258,66 @@
     "_OptionalConversationLevelTestResultItemTypeDef",
     {
         "speechTranscriptionResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
+
 class ConversationLevelTestResultItemTypeDef(
     _RequiredConversationLevelTestResultItemTypeDef, _OptionalConversationLevelTestResultItemTypeDef
 ):
     pass
 
+
 _RequiredTestExecutionResultFilterByTypeDef = TypedDict(
     "_RequiredTestExecutionResultFilterByTypeDef",
     {
         "resultTypeFilter": TestResultTypeFilterType,
     },
 )
 _OptionalTestExecutionResultFilterByTypeDef = TypedDict(
     "_OptionalTestExecutionResultFilterByTypeDef",
     {
         "conversationLevelTestResultsFilterBy": ConversationLevelTestResultsFilterByTypeDef,
     },
     total=False,
 )
 
+
 class TestExecutionResultFilterByTypeDef(
     _RequiredTestExecutionResultFilterByTypeDef, _OptionalTestExecutionResultFilterByTypeDef
 ):
     pass
 
-ConversationLogsDataSourceTypeDef = TypedDict(
-    "ConversationLogsDataSourceTypeDef",
+
+ConversationLogsDataSourceOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceOutputTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
-        "filter": ConversationLogsDataSourceFilterByTypeDef,
+        "filter": ConversationLogsDataSourceFilterByOutputTypeDef,
+    },
+)
+
+ConversationLogsDataSourceFilterByTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "inputMode": ConversationLogsInputModeFilterType,
+    },
+)
+
+DateRangeFilterTypeDef = TypedDict(
+    "DateRangeFilterTypeDef",
+    {
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
     },
 )
 
 IntentSummaryTypeDef = TypedDict(
     "IntentSummaryTypeDef",
     {
         "intentId": str,
@@ -3103,24 +3346,26 @@
     {
         "condition": Mapping[str, Mapping[str, str]],
         "expectedRevisionId": str,
     },
     total=False,
 )
 
+
 class CreateResourcePolicyStatementRequestRequestTypeDef(
     _RequiredCreateResourcePolicyStatementRequestRequestTypeDef,
     _OptionalCreateResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
-LexTranscriptFilterTypeDef = TypedDict(
-    "LexTranscriptFilterTypeDef",
+
+LexTranscriptFilterOutputTypeDef = TypedDict(
+    "LexTranscriptFilterOutputTypeDef",
     {
-        "dateRangeFilter": DateRangeFilterTypeDef,
+        "dateRangeFilter": DateRangeFilterOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     {
@@ -3132,20 +3377,22 @@
     "_OptionalDescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBotAliasRequestBotAliasAvailableWaitTypeDef(
     _RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     _OptionalDescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef = TypedDict(
     "_RequiredDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3154,20 +3401,22 @@
     "_OptionalDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef(
     _RequiredDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     _OptionalDescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3176,20 +3425,22 @@
     "_OptionalDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef(
     _RequiredDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     _OptionalDescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3198,40 +3449,44 @@
     "_OptionalDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef(
     _RequiredDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     _OptionalDescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBotRequestBotAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotRequestBotAvailableWaitTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalDescribeBotRequestBotAvailableWaitTypeDef = TypedDict(
     "_OptionalDescribeBotRequestBotAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBotRequestBotAvailableWaitTypeDef(
     _RequiredDescribeBotRequestBotAvailableWaitTypeDef,
     _OptionalDescribeBotRequestBotAvailableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBotVersionRequestBotVersionAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -3239,60 +3494,66 @@
     "_OptionalDescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBotVersionRequestBotVersionAvailableWaitTypeDef(
     _RequiredDescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     _OptionalDescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeExportRequestBotExportCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeExportRequestBotExportCompletedWaitTypeDef",
     {
         "exportId": str,
     },
 )
 _OptionalDescribeExportRequestBotExportCompletedWaitTypeDef = TypedDict(
     "_OptionalDescribeExportRequestBotExportCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeExportRequestBotExportCompletedWaitTypeDef(
     _RequiredDescribeExportRequestBotExportCompletedWaitTypeDef,
     _OptionalDescribeExportRequestBotExportCompletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImportRequestBotImportCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeImportRequestBotImportCompletedWaitTypeDef",
     {
         "importId": str,
     },
 )
 _OptionalDescribeImportRequestBotImportCompletedWaitTypeDef = TypedDict(
     "_OptionalDescribeImportRequestBotImportCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImportRequestBotImportCompletedWaitTypeDef(
     _RequiredDescribeImportRequestBotImportCompletedWaitTypeDef,
     _OptionalDescribeImportRequestBotImportCompletedWaitTypeDef,
 ):
     pass
 
+
 DescribeBotVersionResponseTypeDef = TypedDict(
     "DescribeBotVersionResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "botVersion": str,
         "description": str,
@@ -3301,15 +3562,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "botType": BotTypeType,
         "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
     "UpdateBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
@@ -3329,15 +3590,15 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestSetSummaryTypeDef = TypedDict(
     "TestSetSummaryTypeDef",
     {
         "testSetId": str,
@@ -3363,16 +3624,26 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DialogStateOutputTypeDef = TypedDict(
+    "DialogStateOutputTypeDef",
+    {
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentOverrideOutputTypeDef,
+        "sessionAttributes": Dict[str, str],
     },
+    total=False,
 )
 
 DialogStateTypeDef = TypedDict(
     "DialogStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentOverrideTypeDef,
@@ -3432,15 +3703,15 @@
     "ListImportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "importSummaries": List[ImportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputSessionStateSpecificationTypeDef = TypedDict(
     "InputSessionStateSpecificationTypeDef",
     {
         "sessionAttributes": Dict[str, str],
@@ -3474,29 +3745,31 @@
         "filters": Sequence[IntentFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListIntentsRequestRequestTypeDef(
     _RequiredListIntentsRequestRequestTypeDef, _OptionalListIntentsRequestRequestTypeDef
 ):
     pass
 
+
 ListRecommendedIntentsResponseTypeDef = TypedDict(
     "ListRecommendedIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotTypesRequestRequestTypeDef",
     {
         "botId": str,
@@ -3511,28 +3784,30 @@
         "filters": Sequence[SlotTypeFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListSlotTypesRequestRequestTypeDef(
     _RequiredListSlotTypesRequestRequestTypeDef, _OptionalListSlotTypesRequestRequestTypeDef
 ):
     pass
 
+
 ListSlotTypesResponseTypeDef = TypedDict(
     "ListSlotTypesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "slotTypeSummaries": List[SlotTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSlotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotsRequestRequestTypeDef",
     {
         "botId": str,
@@ -3548,19 +3823,21 @@
         "filters": Sequence[SlotFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListSlotsRequestRequestTypeDef(
     _RequiredListSlotsRequestRequestTypeDef, _OptionalListSlotsRequestRequestTypeDef
 ):
     pass
 
+
 ListTestExecutionsRequestRequestTypeDef = TypedDict(
     "ListTestExecutionsRequestRequestTypeDef",
     {
         "sortBy": TestExecutionSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
@@ -3596,23 +3873,39 @@
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
+SlotTypeValueOutputTypeDef = TypedDict(
+    "SlotTypeValueOutputTypeDef",
+    {
+        "sampleValue": SampleValueTypeDef,
+        "synonyms": List[SampleValueTypeDef],
+    },
+    total=False,
+)
+
 SlotTypeValueTypeDef = TypedDict(
     "SlotTypeValueTypeDef",
     {
         "sampleValue": SampleValueTypeDef,
         "synonyms": Sequence[SampleValueTypeDef],
     },
     total=False,
 )
 
+SlotDefaultValueSpecificationOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecificationOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueTypeDef],
+    },
+)
+
 SlotDefaultValueSpecificationTypeDef = TypedDict(
     "SlotDefaultValueSpecificationTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
@@ -3620,14 +3913,24 @@
     "SlotResolutionTestResultItemTypeDef",
     {
         "slotName": str,
         "resultCounts": SlotResolutionTestResultItemCountsTypeDef,
     },
 )
 
+SlotValueOverrideOutputTypeDef = TypedDict(
+    "SlotValueOverrideOutputTypeDef",
+    {
+        "shape": SlotShapeType,
+        "value": SlotValueTypeDef,
+        "values": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 SlotValueOverrideTypeDef = TypedDict(
     "SlotValueOverrideTypeDef",
     {
         "shape": SlotShapeType,
         "value": SlotValueTypeDef,
         "values": Sequence[Dict[str, Any]],
     },
@@ -3645,19 +3948,21 @@
     {
         "regexFilter": SlotValueRegexFilterTypeDef,
         "advancedRecognitionSetting": AdvancedRecognitionSettingTypeDef,
     },
     total=False,
 )
 
+
 class SlotValueSelectionSettingTypeDef(
     _RequiredSlotValueSelectionSettingTypeDef, _OptionalSlotValueSelectionSettingTypeDef
 ):
     pass
 
+
 TestSetDiscrepancyErrorsTypeDef = TypedDict(
     "TestSetDiscrepancyErrorsTypeDef",
     {
         "intentDiscrepancies": List[TestSetIntentDiscrepancyItemTypeDef],
         "slotDiscrepancies": List[TestSetSlotDiscrepancyItemTypeDef],
     },
 )
@@ -3666,39 +3971,68 @@
     "TestSetDiscrepancyReportResourceTargetTypeDef",
     {
         "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetTypeDef,
     },
     total=False,
 )
 
+_RequiredTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
+    "_RequiredTestSetImportResourceSpecificationOutputTypeDef",
+    {
+        "testSetName": str,
+        "roleArn": str,
+        "storageLocation": TestSetStorageLocationTypeDef,
+        "importInputLocation": TestSetImportInputLocationTypeDef,
+        "modality": TestSetModalityType,
+    },
+)
+_OptionalTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
+    "_OptionalTestSetImportResourceSpecificationOutputTypeDef",
+    {
+        "description": str,
+        "testSetTags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class TestSetImportResourceSpecificationOutputTypeDef(
+    _RequiredTestSetImportResourceSpecificationOutputTypeDef,
+    _OptionalTestSetImportResourceSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_RequiredTestSetImportResourceSpecificationTypeDef",
     {
         "testSetName": str,
         "roleArn": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "importInputLocation": TestSetImportInputLocationTypeDef,
         "modality": TestSetModalityType,
     },
 )
 _OptionalTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_OptionalTestSetImportResourceSpecificationTypeDef",
     {
         "description": str,
-        "testSetTags": Dict[str, str],
+        "testSetTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TestSetImportResourceSpecificationTypeDef(
     _RequiredTestSetImportResourceSpecificationTypeDef,
     _OptionalTestSetImportResourceSpecificationTypeDef,
 ):
     pass
 
+
 _RequiredUserTurnOutputSpecificationTypeDef = TypedDict(
     "_RequiredUserTurnOutputSpecificationTypeDef",
     {
         "intent": UserTurnIntentOutputTypeDef,
     },
 )
 _OptionalUserTurnOutputSpecificationTypeDef = TypedDict(
@@ -3706,19 +4040,21 @@
     {
         "activeContexts": List[ActiveContextTypeDef],
         "transcript": str,
     },
     total=False,
 )
 
+
 class UserTurnOutputSpecificationTypeDef(
     _RequiredUserTurnOutputSpecificationTypeDef, _OptionalUserTurnOutputSpecificationTypeDef
 ):
     pass
 
+
 UtteranceInputSpecificationTypeDef = TypedDict(
     "UtteranceInputSpecificationTypeDef",
     {
         "textInput": str,
         "audioInput": UtteranceAudioInputSpecificationTypeDef,
     },
     total=False,
@@ -3736,19 +4072,21 @@
         "allowInterrupt": bool,
         "audioAndDTMFInputSpecification": AudioAndDTMFInputSpecificationTypeDef,
         "textInputSpecification": TextInputSpecificationTypeDef,
     },
     total=False,
 )
 
+
 class PromptAttemptSpecificationTypeDef(
     _RequiredPromptAttemptSpecificationTypeDef, _OptionalPromptAttemptSpecificationTypeDef
 ):
     pass
 
+
 AudioLogSettingTypeDef = TypedDict(
     "AudioLogSettingTypeDef",
     {
         "enabled": bool,
         "destination": AudioLogDestinationTypeDef,
     },
 )
@@ -3762,15 +4100,15 @@
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
         "target": TestExecutionTargetTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartTestExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestExecutionRequestRequestTypeDef",
     {
         "testSetId": str,
@@ -3782,30 +4120,32 @@
     "_OptionalStartTestExecutionRequestRequestTypeDef",
     {
         "testExecutionModality": TestExecutionModalityType,
     },
     total=False,
 )
 
+
 class StartTestExecutionRequestRequestTypeDef(
     _RequiredStartTestExecutionRequestRequestTypeDef,
     _OptionalStartTestExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 StartTestExecutionResponseTypeDef = TypedDict(
     "StartTestExecutionResponseTypeDef",
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestExecutionTargetTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionSummaryTypeDef = TypedDict(
     "TestExecutionSummaryTypeDef",
     {
         "testExecutionId": str,
@@ -3827,14 +4167,25 @@
         "botLocaleExportUrl": str,
         "associatedTranscriptsUrl": str,
         "statistics": BotRecommendationResultStatisticsTypeDef,
     },
     total=False,
 )
 
+MessageOutputTypeDef = TypedDict(
+    "MessageOutputTypeDef",
+    {
+        "plainTextMessage": PlainTextMessageTypeDef,
+        "customPayload": CustomPayloadTypeDef,
+        "ssmlMessage": SSMLMessageTypeDef,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
+    total=False,
+)
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "plainTextMessage": PlainTextMessageTypeDef,
         "customPayload": CustomPayloadTypeDef,
         "ssmlMessage": SSMLMessageTypeDef,
         "imageResponseCard": ImageResponseCardTypeDef,
@@ -3860,19 +4211,24 @@
     "_OptionalBotAliasLocaleSettingsTypeDef",
     {
         "codeHookSpecification": CodeHookSpecificationTypeDef,
     },
     total=False,
 )
 
+
 class BotAliasLocaleSettingsTypeDef(
     _RequiredBotAliasLocaleSettingsTypeDef, _OptionalBotAliasLocaleSettingsTypeDef
 ):
     pass
 
+
+CompositeSlotTypeSettingUnionTypeDef = Union[
+    CompositeSlotTypeSettingTypeDef, CompositeSlotTypeSettingOutputTypeDef
+]
 ConversationLevelTestResultsTypeDef = TypedDict(
     "ConversationLevelTestResultsTypeDef",
     {
         "items": List[ConversationLevelTestResultItemTypeDef],
     },
 )
 
@@ -3888,54 +4244,74 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTestExecutionResultItemsRequestRequestTypeDef(
     _RequiredListTestExecutionResultItemsRequestRequestTypeDef,
     _OptionalListTestExecutionResultItemsRequestRequestTypeDef,
 ):
     pass
 
-TestSetGenerationDataSourceTypeDef = TypedDict(
-    "TestSetGenerationDataSourceTypeDef",
+
+TestSetGenerationDataSourceOutputTypeDef = TypedDict(
+    "TestSetGenerationDataSourceOutputTypeDef",
     {
-        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
+        "conversationLogsDataSource": ConversationLogsDataSourceOutputTypeDef,
+    },
+    total=False,
+)
+
+ConversationLogsDataSourceTypeDef = TypedDict(
+    "ConversationLogsDataSourceTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "filter": ConversationLogsDataSourceFilterByTypeDef,
+    },
+)
+
+LexTranscriptFilterTypeDef = TypedDict(
+    "LexTranscriptFilterTypeDef",
+    {
+        "dateRangeFilter": DateRangeFilterTypeDef,
     },
     total=False,
 )
 
 ListIntentsResponseTypeDef = TypedDict(
     "ListIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TranscriptFilterTypeDef = TypedDict(
-    "TranscriptFilterTypeDef",
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
-        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
+        "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
     },
     total=False,
 )
 
 ListTestSetsResponseTypeDef = TypedDict(
     "ListTestSetsResponseTypeDef",
     {
         "testSets": List[TestSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExportRequestRequestTypeDef",
     {
         "resourceSpecification": ExportResourceSpecificationTypeDef,
@@ -3946,43 +4322,45 @@
     "_OptionalCreateExportRequestRequestTypeDef",
     {
         "filePassword": str,
     },
     total=False,
 )
 
+
 class CreateExportRequestRequestTypeDef(
     _RequiredCreateExportRequestRequestTypeDef, _OptionalCreateExportRequestRequestTypeDef
 ):
     pass
 
+
 CreateExportResponseTypeDef = TypedDict(
     "CreateExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportResponseTypeDef = TypedDict(
     "DescribeExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "failureReasons": List[str],
         "downloadUrl": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "exportId": str,
@@ -4000,15 +4378,15 @@
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExternalSourceSettingTypeDef = TypedDict(
     "ExternalSourceSettingTypeDef",
     {
         "grammarSlotTypeSetting": GrammarSlotTypeSettingTypeDef,
@@ -4040,37 +4418,40 @@
         "filters": Sequence[AggregatedUtterancesFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListAggregatedUtterancesRequestRequestTypeDef(
     _RequiredListAggregatedUtterancesRequestRequestTypeDef,
     _OptionalListAggregatedUtterancesRequestRequestTypeDef,
 ):
     pass
 
+
 ListAggregatedUtterancesResponseTypeDef = TypedDict(
     "ListAggregatedUtterancesResponseTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "botVersion": str,
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationTypeDef,
         "aggregationWindowStartTime": datetime,
         "aggregationWindowEndTime": datetime,
         "aggregationLastRefreshedDateTime": datetime,
         "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SlotTypeValueUnionTypeDef = Union[SlotTypeValueTypeDef, SlotTypeValueOutputTypeDef]
 IntentLevelSlotResolutionTestResultItemTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
         "slotResolutionResults": List[SlotResolutionTestResultItemTypeDef],
     },
@@ -4087,15 +4468,15 @@
 CreateTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestSetDiscrepancyReportResourceTargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
@@ -4103,18 +4484,29 @@
         "creationDateTime": datetime,
         "target": TestSetDiscrepancyReportResourceTargetTypeDef,
         "testSetDiscrepancyReportStatus": TestSetDiscrepancyReportStatusType,
         "lastUpdatedDataTime": datetime,
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportResourceSpecificationOutputTypeDef = TypedDict(
+    "ImportResourceSpecificationOutputTypeDef",
+    {
+        "botImportSpecification": BotImportSpecificationOutputTypeDef,
+        "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
+        "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
+        "testSetImportResourceSpecification": TestSetImportResourceSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImportResourceSpecificationTypeDef = TypedDict(
     "ImportResourceSpecificationTypeDef",
     {
         "botImportSpecification": BotImportSpecificationTypeDef,
         "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
         "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
         "testSetImportResourceSpecification": TestSetImportResourceSpecificationTypeDef,
@@ -4133,45 +4525,79 @@
     {
         "requestAttributes": Dict[str, str],
         "sessionState": InputSessionStateSpecificationTypeDef,
     },
     total=False,
 )
 
+
 class UserTurnInputSpecificationTypeDef(
     _RequiredUserTurnInputSpecificationTypeDef, _OptionalUserTurnInputSpecificationTypeDef
 ):
     pass
 
+
 ListTestExecutionsResponseTypeDef = TypedDict(
     "ListTestExecutionsResponseTypeDef",
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredMessageGroupOutputTypeDef = TypedDict(
+    "_RequiredMessageGroupOutputTypeDef",
+    {
+        "message": MessageOutputTypeDef,
+    },
+)
+_OptionalMessageGroupOutputTypeDef = TypedDict(
+    "_OptionalMessageGroupOutputTypeDef",
+    {
+        "variations": List[MessageOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class MessageGroupOutputTypeDef(
+    _RequiredMessageGroupOutputTypeDef, _OptionalMessageGroupOutputTypeDef
+):
+    pass
+
+
 _RequiredMessageGroupTypeDef = TypedDict(
     "_RequiredMessageGroupTypeDef",
     {
         "message": MessageTypeDef,
     },
 )
 _OptionalMessageGroupTypeDef = TypedDict(
     "_OptionalMessageGroupTypeDef",
     {
         "variations": Sequence[MessageTypeDef],
     },
     total=False,
 )
 
+
 class MessageGroupTypeDef(_RequiredMessageGroupTypeDef, _OptionalMessageGroupTypeDef):
     pass
 
+
+ConversationLogSettingsOutputTypeDef = TypedDict(
+    "ConversationLogSettingsOutputTypeDef",
+    {
+        "textLogSettings": List[TextLogSettingTypeDef],
+        "audioLogSettings": List[AudioLogSettingTypeDef],
+    },
+    total=False,
+)
+
 ConversationLogSettingsTypeDef = TypedDict(
     "ConversationLogSettingsTypeDef",
     {
         "textLogSettings": Sequence[TextLogSettingTypeDef],
         "audioLogSettings": Sequence[AudioLogSettingTypeDef],
     },
     total=False,
@@ -4183,233 +4609,246 @@
         "testSetGenerationId": str,
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "failureReasons": List[str],
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
+StartTestSetGenerationResponseTypeDef = TypedDict(
+    "StartTestSetGenerationResponseTypeDef",
     {
+        "testSetGenerationId": str,
+        "creationDateTime": datetime,
+        "testSetGenerationStatus": TestSetGenerationStatusType,
         "testSetName": str,
+        "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
+        "testSetTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
+
+TestSetGenerationDataSourceTypeDef = TypedDict(
+    "TestSetGenerationDataSourceTypeDef",
     {
-        "description": str,
-        "testSetTags": Mapping[str, str],
+        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
     },
     total=False,
 )
 
-class StartTestSetGenerationRequestRequestTypeDef(
-    _RequiredStartTestSetGenerationRequestRequestTypeDef,
-    _OptionalStartTestSetGenerationRequestRequestTypeDef,
-):
-    pass
-
-StartTestSetGenerationResponseTypeDef = TypedDict(
-    "StartTestSetGenerationResponseTypeDef",
+TranscriptFilterTypeDef = TypedDict(
+    "TranscriptFilterTypeDef",
     {
-        "testSetGenerationId": str,
-        "creationDateTime": datetime,
-        "testSetGenerationStatus": TestSetGenerationStatusType,
-        "testSetName": str,
-        "description": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
-        "roleArn": str,
-        "testSetTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
     },
+    total=False,
 )
 
-_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_RequiredS3BucketTranscriptSourceTypeDef",
+_RequiredS3BucketTranscriptSourceOutputTypeDef = TypedDict(
+    "_RequiredS3BucketTranscriptSourceOutputTypeDef",
     {
         "s3BucketName": str,
         "transcriptFormat": Literal["Lex"],
     },
 )
-_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_OptionalS3BucketTranscriptSourceTypeDef",
+_OptionalS3BucketTranscriptSourceOutputTypeDef = TypedDict(
+    "_OptionalS3BucketTranscriptSourceOutputTypeDef",
     {
-        "pathFormat": PathFormatTypeDef,
-        "transcriptFilter": TranscriptFilterTypeDef,
+        "pathFormat": PathFormatOutputTypeDef,
+        "transcriptFilter": TranscriptFilterOutputTypeDef,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-class S3BucketTranscriptSourceTypeDef(
-    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
+
+class S3BucketTranscriptSourceOutputTypeDef(
+    _RequiredS3BucketTranscriptSourceOutputTypeDef, _OptionalS3BucketTranscriptSourceOutputTypeDef
 ):
     pass
 
+
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotTypeRequestRequestTypeDef",
+CreateSlotTypeResponseTypeDef = TypedDict(
+    "CreateSlotTypeResponseTypeDef",
     {
+        "slotTypeId": str,
         "slotTypeName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotTypeRequestRequestTypeDef",
-    {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateSlotTypeRequestRequestTypeDef(
-    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
-):
-    pass
-
-CreateSlotTypeResponseTypeDef = TypedDict(
-    "CreateSlotTypeResponseTypeDef",
+DescribeSlotTypeResponseTypeDef = TypedDict(
+    "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSlotTypeResponseTypeDef = TypedDict(
-    "DescribeSlotTypeResponseTypeDef",
+UpdateSlotTypeResponseTypeDef = TypedDict(
+    "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
+_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
-        "slotTypeId": str,
         "slotTypeName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
     total=False,
 )
 
-class UpdateSlotTypeRequestRequestTypeDef(
-    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+
+class CreateSlotTypeRequestRequestTypeDef(
+    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
 ):
     pass
 
-UpdateSlotTypeResponseTypeDef = TypedDict(
-    "UpdateSlotTypeResponseTypeDef",
+
+_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
-        "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+
+class UpdateSlotTypeRequestRequestTypeDef(
+    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+):
+    pass
+
+
 IntentLevelSlotResolutionTestResultsTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultsTypeDef",
     {
         "items": List[IntentLevelSlotResolutionTestResultItemTypeDef],
     },
 )
 
 DescribeImportResponseTypeDef = TypedDict(
     "DescribeImportResponseTypeDef",
     {
         "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
+    {
+        "importId": str,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
+        "mergeStrategy": MergeStrategyType,
+        "importStatus": ImportStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportResourceSpecificationUnionTypeDef = Union[
+    ImportResourceSpecificationTypeDef, ImportResourceSpecificationOutputTypeDef
+]
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationTypeDef,
         "mergeStrategy": MergeStrategyType,
     },
@@ -4418,30 +4857,20 @@
     "_OptionalStartImportRequestRequestTypeDef",
     {
         "filePassword": str,
     },
     total=False,
 )
 
+
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
-    {
-        "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
-        "mergeStrategy": MergeStrategyType,
-        "importStatus": ImportStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUserTurnResultTypeDef = TypedDict(
     "_RequiredUserTurnResultTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expectedOutput": UserTurnOutputSpecificationTypeDef,
     },
@@ -4456,25 +4885,142 @@
         "slotMatchResult": TestResultMatchStatusType,
         "speechTranscriptionResult": TestResultMatchStatusType,
         "conversationLevelResult": ConversationLevelResultDetailTypeDef,
     },
     total=False,
 )
 
+
 class UserTurnResultTypeDef(_RequiredUserTurnResultTypeDef, _OptionalUserTurnResultTypeDef):
     pass
 
+
 UserTurnSpecificationTypeDef = TypedDict(
     "UserTurnSpecificationTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expected": UserTurnOutputSpecificationTypeDef,
     },
 )
 
+_RequiredFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentStartResponseSpecificationOutputTypeDef",
+    {
+        "delayInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+    },
+)
+_OptionalFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentStartResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+
+class FulfillmentStartResponseSpecificationOutputTypeDef(
+    _RequiredFulfillmentStartResponseSpecificationOutputTypeDef,
+    _OptionalFulfillmentStartResponseSpecificationOutputTypeDef,
+):
+    pass
+
+
+_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef",
+    {
+        "frequencyInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+    },
+)
+_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+
+class FulfillmentUpdateResponseSpecificationOutputTypeDef(
+    _RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef,
+    _OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef,
+):
+    pass
+
+
+_RequiredPromptSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPromptSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "maxRetries": int,
+    },
+)
+_OptionalPromptSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPromptSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+        "messageSelectionStrategy": MessageSelectionStrategyType,
+        "promptAttemptsSpecification": Dict[PromptAttemptType, PromptAttemptSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class PromptSpecificationOutputTypeDef(
+    _RequiredPromptSpecificationOutputTypeDef, _OptionalPromptSpecificationOutputTypeDef
+):
+    pass
+
+
+_RequiredResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+    },
+)
+_OptionalResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+
+class ResponseSpecificationOutputTypeDef(
+    _RequiredResponseSpecificationOutputTypeDef, _OptionalResponseSpecificationOutputTypeDef
+):
+    pass
+
+
+_RequiredStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredStillWaitingResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "frequencyInSeconds": int,
+        "timeoutInSeconds": int,
+    },
+)
+_OptionalStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalStillWaitingResponseSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+    },
+    total=False,
+)
+
+
+class StillWaitingResponseSpecificationOutputTypeDef(
+    _RequiredStillWaitingResponseSpecificationOutputTypeDef,
+    _OptionalStillWaitingResponseSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4482,20 +5028,22 @@
     "_OptionalFulfillmentStartResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
+
 class FulfillmentStartResponseSpecificationTypeDef(
     _RequiredFulfillmentStartResponseSpecificationTypeDef,
     _OptionalFulfillmentStartResponseSpecificationTypeDef,
 ):
     pass
 
+
 _RequiredFulfillmentUpdateResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentUpdateResponseSpecificationTypeDef",
     {
         "frequencyInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4503,20 +5051,22 @@
     "_OptionalFulfillmentUpdateResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
+
 class FulfillmentUpdateResponseSpecificationTypeDef(
     _RequiredFulfillmentUpdateResponseSpecificationTypeDef,
     _OptionalFulfillmentUpdateResponseSpecificationTypeDef,
 ):
     pass
 
+
 _RequiredPromptSpecificationTypeDef = TypedDict(
     "_RequiredPromptSpecificationTypeDef",
     {
         "messageGroups": Sequence[MessageGroupTypeDef],
         "maxRetries": int,
     },
 )
@@ -4528,38 +5078,42 @@
         "promptAttemptsSpecification": Mapping[
             PromptAttemptType, PromptAttemptSpecificationTypeDef
         ],
     },
     total=False,
 )
 
+
 class PromptSpecificationTypeDef(
     _RequiredPromptSpecificationTypeDef, _OptionalPromptSpecificationTypeDef
 ):
     pass
 
+
 _RequiredResponseSpecificationTypeDef = TypedDict(
     "_RequiredResponseSpecificationTypeDef",
     {
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
 _OptionalResponseSpecificationTypeDef = TypedDict(
     "_OptionalResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
+
 class ResponseSpecificationTypeDef(
     _RequiredResponseSpecificationTypeDef, _OptionalResponseSpecificationTypeDef
 ):
     pass
 
+
 _RequiredStillWaitingResponseSpecificationTypeDef = TypedDict(
     "_RequiredStillWaitingResponseSpecificationTypeDef",
     {
         "messageGroups": Sequence[MessageGroupTypeDef],
         "frequencyInSeconds": int,
         "timeoutInSeconds": int,
     },
@@ -4568,83 +5122,108 @@
     "_OptionalStillWaitingResponseSpecificationTypeDef",
     {
         "allowInterrupt": bool,
     },
     total=False,
 )
 
+
 class StillWaitingResponseSpecificationTypeDef(
     _RequiredStillWaitingResponseSpecificationTypeDef,
     _OptionalStillWaitingResponseSpecificationTypeDef,
 ):
     pass
 
-_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotAliasRequestRequestTypeDef",
-    {
-        "botAliasName": str,
-        "botId": str,
-    },
-)
-_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotAliasRequestRequestTypeDef",
-    {
-        "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateBotAliasRequestRequestTypeDef(
-    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
-):
-    pass
 
 CreateBotAliasResponseTypeDef = TypedDict(
     "CreateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotAliasResponseTypeDef = TypedDict(
     "DescribeBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBotAliasResponseTypeDef = TypedDict(
+    "UpdateBotAliasResponseTypeDef",
+    {
+        "botAliasId": str,
+        "botAliasName": str,
+        "description": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasStatus": BotAliasStatusType,
+        "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConversationLogSettingsUnionTypeDef = Union[
+    ConversationLogSettingsTypeDef, ConversationLogSettingsOutputTypeDef
+]
+_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotAliasRequestRequestTypeDef",
+    {
+        "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotAliasRequestRequestTypeDef",
+    {
+        "description": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateBotAliasRequestRequestTypeDef(
+    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "botId": str,
     },
@@ -4657,41 +5236,78 @@
         "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBotAliasRequestRequestTypeDef(
     _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
 ):
     pass
 
-UpdateBotAliasResponseTypeDef = TypedDict(
-    "UpdateBotAliasResponseTypeDef",
+
+_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
+    {
+        "testSetName": str,
+        "storageLocation": TestSetStorageLocationTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "roleArn": str,
+    },
+)
+_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
     {
-        "botAliasId": str,
-        "botAliasName": str,
         "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasStatus": BotAliasStatusType,
-        "botId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "testSetTags": Mapping[str, str],
     },
+    total=False,
 )
 
-TranscriptSourceSettingTypeDef = TypedDict(
-    "TranscriptSourceSettingTypeDef",
+
+class StartTestSetGenerationRequestRequestTypeDef(
+    _RequiredStartTestSetGenerationRequestRequestTypeDef,
+    _OptionalStartTestSetGenerationRequestRequestTypeDef,
+):
+    pass
+
+
+TestSetGenerationDataSourceUnionTypeDef = Union[
+    TestSetGenerationDataSourceTypeDef, TestSetGenerationDataSourceOutputTypeDef
+]
+_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_RequiredS3BucketTranscriptSourceTypeDef",
     {
-        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
+        "s3BucketName": str,
+        "transcriptFormat": Literal["Lex"],
+    },
+)
+_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_OptionalS3BucketTranscriptSourceTypeDef",
+    {
+        "pathFormat": PathFormatTypeDef,
+        "transcriptFilter": TranscriptFilterTypeDef,
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+
+class S3BucketTranscriptSourceTypeDef(
+    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
+):
+    pass
+
+
+TranscriptSourceSettingOutputTypeDef = TypedDict(
+    "TranscriptSourceSettingOutputTypeDef",
+    {
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceOutputTypeDef,
     },
     total=False,
 )
 
 TestSetTurnResultTypeDef = TypedDict(
     "TestSetTurnResultTypeDef",
     {
@@ -4706,49 +5322,131 @@
     {
         "agentTurn": AgentTurnSpecificationTypeDef,
         "userTurn": UserTurnSpecificationTypeDef,
     },
     total=False,
 )
 
-_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
+_RequiredFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdatesSpecificationOutputTypeDef",
     {
         "active": bool,
     },
 )
-_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
+_OptionalFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdatesSpecificationOutputTypeDef",
     {
-        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
-        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
+        "startResponse": FulfillmentStartResponseSpecificationOutputTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationOutputTypeDef,
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
-class FulfillmentUpdatesSpecificationTypeDef(
-    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
+
+class FulfillmentUpdatesSpecificationOutputTypeDef(
+    _RequiredFulfillmentUpdatesSpecificationOutputTypeDef,
+    _OptionalFulfillmentUpdatesSpecificationOutputTypeDef,
 ):
     pass
 
+
 SlotSummaryTypeDef = TypedDict(
     "SlotSummaryTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotConstraint": SlotConstraintType,
         "slotTypeId": str,
-        "valueElicitationPromptSpecification": PromptSpecificationTypeDef,
+        "valueElicitationPromptSpecification": PromptSpecificationOutputTypeDef,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+_RequiredConditionalBranchOutputTypeDef = TypedDict(
+    "_RequiredConditionalBranchOutputTypeDef",
+    {
+        "name": str,
+        "condition": ConditionTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+    },
+)
+_OptionalConditionalBranchOutputTypeDef = TypedDict(
+    "_OptionalConditionalBranchOutputTypeDef",
+    {
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ConditionalBranchOutputTypeDef(
+    _RequiredConditionalBranchOutputTypeDef, _OptionalConditionalBranchOutputTypeDef
+):
+    pass
+
+
+DefaultConditionalBranchOutputTypeDef = TypedDict(
+    "DefaultConditionalBranchOutputTypeDef",
+    {
+        "nextStep": DialogStateOutputTypeDef,
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredWaitAndContinueSpecificationOutputTypeDef = TypedDict(
+    "_RequiredWaitAndContinueSpecificationOutputTypeDef",
+    {
+        "waitingResponse": ResponseSpecificationOutputTypeDef,
+        "continueResponse": ResponseSpecificationOutputTypeDef,
+    },
+)
+_OptionalWaitAndContinueSpecificationOutputTypeDef = TypedDict(
+    "_OptionalWaitAndContinueSpecificationOutputTypeDef",
+    {
+        "stillWaitingResponse": StillWaitingResponseSpecificationOutputTypeDef,
+        "active": bool,
+    },
+    total=False,
+)
+
+
+class WaitAndContinueSpecificationOutputTypeDef(
+    _RequiredWaitAndContinueSpecificationOutputTypeDef,
+    _OptionalWaitAndContinueSpecificationOutputTypeDef,
+):
+    pass
+
+
+_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
+    {
+        "active": bool,
+    },
+)
+_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
+    {
+        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
+        "timeoutInSeconds": int,
+    },
+    total=False,
+)
+
+
+class FulfillmentUpdatesSpecificationTypeDef(
+    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
+):
+    pass
+
+
 _RequiredConditionalBranchTypeDef = TypedDict(
     "_RequiredConditionalBranchTypeDef",
     {
         "name": str,
         "condition": ConditionTypeDef,
         "nextStep": DialogStateTypeDef,
     },
@@ -4757,19 +5455,21 @@
     "_OptionalConditionalBranchTypeDef",
     {
         "response": ResponseSpecificationTypeDef,
     },
     total=False,
 )
 
+
 class ConditionalBranchTypeDef(
     _RequiredConditionalBranchTypeDef, _OptionalConditionalBranchTypeDef
 ):
     pass
 
+
 DefaultConditionalBranchTypeDef = TypedDict(
     "DefaultConditionalBranchTypeDef",
     {
         "nextStep": DialogStateTypeDef,
         "response": ResponseSpecificationTypeDef,
     },
     total=False,
@@ -4787,88 +5487,75 @@
     {
         "stillWaitingResponse": StillWaitingResponseSpecificationTypeDef,
         "active": bool,
     },
     total=False,
 )
 
+
 class WaitAndContinueSpecificationTypeDef(
     _RequiredWaitAndContinueSpecificationTypeDef, _OptionalWaitAndContinueSpecificationTypeDef
 ):
     pass
 
+
+TranscriptSourceSettingTypeDef = TypedDict(
+    "TranscriptSourceSettingTypeDef",
+    {
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
+    },
+    total=False,
+)
+
 DescribeBotRecommendationResponseTypeDef = TypedDict(
     "DescribeBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-    },
-)
-_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartBotRecommendationRequestRequestTypeDef",
-    {
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-    total=False,
-)
-
-class StartBotRecommendationRequestRequestTypeDef(
-    _RequiredStartBotRecommendationRequestRequestTypeDef,
-    _OptionalStartBotRecommendationRequestRequestTypeDef,
-):
-    pass
-
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUtteranceLevelTestResultItemTypeDef = TypedDict(
     "_RequiredUtteranceLevelTestResultItemTypeDef",
     {
         "recordNumber": int,
@@ -4879,19 +5566,21 @@
     "_OptionalUtteranceLevelTestResultItemTypeDef",
     {
         "conversationId": str,
     },
     total=False,
 )
 
+
 class UtteranceLevelTestResultItemTypeDef(
     _RequiredUtteranceLevelTestResultItemTypeDef, _OptionalUtteranceLevelTestResultItemTypeDef
 ):
     pass
 
+
 _RequiredTestSetTurnRecordTypeDef = TypedDict(
     "_RequiredTestSetTurnRecordTypeDef",
     {
         "recordNumber": int,
         "turnSpecification": TurnSpecificationTypeDef,
     },
 )
@@ -4900,31 +5589,66 @@
     {
         "conversationId": str,
         "turnNumber": int,
     },
     total=False,
 )
 
+
 class TestSetTurnRecordTypeDef(
     _RequiredTestSetTurnRecordTypeDef, _OptionalTestSetTurnRecordTypeDef
 ):
     pass
 
+
 ListSlotsResponseTypeDef = TypedDict(
     "ListSlotsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConditionalSpecificationOutputTypeDef = TypedDict(
+    "ConditionalSpecificationOutputTypeDef",
+    {
+        "active": bool,
+        "conditionalBranches": List[ConditionalBranchOutputTypeDef],
+        "defaultBranch": DefaultConditionalBranchOutputTypeDef,
+    },
+)
+
+_RequiredSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_RequiredSubSlotValueElicitationSettingOutputTypeDef",
+    {
+        "promptSpecification": PromptSpecificationOutputTypeDef,
     },
 )
+_OptionalSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_OptionalSubSlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SubSlotValueElicitationSettingOutputTypeDef(
+    _RequiredSubSlotValueElicitationSettingOutputTypeDef,
+    _OptionalSubSlotValueElicitationSettingOutputTypeDef,
+):
+    pass
+
 
 ConditionalSpecificationTypeDef = TypedDict(
     "ConditionalSpecificationTypeDef",
     {
         "active": bool,
         "conditionalBranches": Sequence[ConditionalBranchTypeDef],
         "defaultBranch": DefaultConditionalBranchTypeDef,
@@ -4943,32 +5667,113 @@
         "defaultValueSpecification": SlotDefaultValueSpecificationTypeDef,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "waitAndContinueSpecification": WaitAndContinueSpecificationTypeDef,
     },
     total=False,
 )
 
+
 class SubSlotValueElicitationSettingTypeDef(
     _RequiredSubSlotValueElicitationSettingTypeDef, _OptionalSubSlotValueElicitationSettingTypeDef
 ):
     pass
 
+
+_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartBotRecommendationRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+    },
+)
+_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartBotRecommendationRequestRequestTypeDef",
+    {
+        "encryptionSetting": EncryptionSettingTypeDef,
+    },
+    total=False,
+)
+
+
+class StartBotRecommendationRequestRequestTypeDef(
+    _RequiredStartBotRecommendationRequestRequestTypeDef,
+    _OptionalStartBotRecommendationRequestRequestTypeDef,
+):
+    pass
+
+
+TranscriptSourceSettingUnionTypeDef = Union[
+    TranscriptSourceSettingTypeDef, TranscriptSourceSettingOutputTypeDef
+]
 UtteranceLevelTestResultsTypeDef = TypedDict(
     "UtteranceLevelTestResultsTypeDef",
     {
         "items": List[UtteranceLevelTestResultItemTypeDef],
     },
 )
 
 ListTestSetRecordsResponseTypeDef = TypedDict(
     "ListTestSetRecordsResponseTypeDef",
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IntentClosingSettingOutputTypeDef = TypedDict(
+    "IntentClosingSettingOutputTypeDef",
+    {
+        "closingResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+PostDialogCodeHookInvocationSpecificationOutputTypeDef = TypedDict(
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+PostFulfillmentStatusSpecificationOutputTypeDef = TypedDict(
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+SpecificationsOutputTypeDef = TypedDict(
+    "SpecificationsOutputTypeDef",
+    {
+        "slotTypeId": str,
+        "valueElicitationSetting": SubSlotValueElicitationSettingOutputTypeDef,
     },
 )
 
 IntentClosingSettingTypeDef = TypedDict(
     "IntentClosingSettingTypeDef",
     {
         "closingResponse": ResponseSpecificationTypeDef,
@@ -5027,14 +5832,74 @@
         "intentClassificationTestResults": IntentClassificationTestResultsTypeDef,
         "intentLevelSlotResolutionTestResults": IntentLevelSlotResolutionTestResultsTypeDef,
         "utteranceLevelTestResults": UtteranceLevelTestResultsTypeDef,
     },
     total=False,
 )
 
+_RequiredDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "_RequiredDialogCodeHookInvocationSettingOutputTypeDef",
+    {
+        "enableCodeHookInvocation": bool,
+        "active": bool,
+        "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    },
+)
+_OptionalDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "_OptionalDialogCodeHookInvocationSettingOutputTypeDef",
+    {
+        "invocationLabel": str,
+    },
+    total=False,
+)
+
+
+class DialogCodeHookInvocationSettingOutputTypeDef(
+    _RequiredDialogCodeHookInvocationSettingOutputTypeDef,
+    _OptionalDialogCodeHookInvocationSettingOutputTypeDef,
+):
+    pass
+
+
+_RequiredFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentCodeHookSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentCodeHookSettingsOutputTypeDef",
+    {
+        "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationOutputTypeDef,
+        "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationOutputTypeDef,
+        "active": bool,
+    },
+    total=False,
+)
+
+
+class FulfillmentCodeHookSettingsOutputTypeDef(
+    _RequiredFulfillmentCodeHookSettingsOutputTypeDef,
+    _OptionalFulfillmentCodeHookSettingsOutputTypeDef,
+):
+    pass
+
+
+SubSlotSettingOutputTypeDef = TypedDict(
+    "SubSlotSettingOutputTypeDef",
+    {
+        "expression": str,
+        "slotSpecifications": Dict[str, SpecificationsOutputTypeDef],
+    },
+    total=False,
+)
+
+IntentClosingSettingUnionTypeDef = Union[
+    IntentClosingSettingTypeDef, IntentClosingSettingOutputTypeDef
+]
 _RequiredDialogCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredDialogCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
         "active": bool,
         "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationTypeDef,
     },
@@ -5043,19 +5908,21 @@
     "_OptionalDialogCodeHookInvocationSettingTypeDef",
     {
         "invocationLabel": str,
     },
     total=False,
 )
 
+
 class DialogCodeHookInvocationSettingTypeDef(
     _RequiredDialogCodeHookInvocationSettingTypeDef, _OptionalDialogCodeHookInvocationSettingTypeDef
 ):
     pass
 
+
 _RequiredFulfillmentCodeHookSettingsTypeDef = TypedDict(
     "_RequiredFulfillmentCodeHookSettingsTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalFulfillmentCodeHookSettingsTypeDef = TypedDict(
@@ -5064,35 +5931,95 @@
         "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationTypeDef,
         "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationTypeDef,
         "active": bool,
     },
     total=False,
 )
 
+
 class FulfillmentCodeHookSettingsTypeDef(
     _RequiredFulfillmentCodeHookSettingsTypeDef, _OptionalFulfillmentCodeHookSettingsTypeDef
 ):
     pass
 
+
 SubSlotSettingTypeDef = TypedDict(
     "SubSlotSettingTypeDef",
     {
         "expression": str,
         "slotSpecifications": Mapping[str, SpecificationsTypeDef],
     },
     total=False,
 )
 
 ListTestExecutionResultItemsResponseTypeDef = TypedDict(
     "ListTestExecutionResultItemsResponseTypeDef",
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitialResponseSettingOutputTypeDef = TypedDict(
+    "InitialResponseSettingOutputTypeDef",
+    {
+        "initialResponse": ResponseSpecificationOutputTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredIntentConfirmationSettingOutputTypeDef = TypedDict(
+    "_RequiredIntentConfirmationSettingOutputTypeDef",
+    {
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+    },
+)
+_OptionalIntentConfirmationSettingOutputTypeDef = TypedDict(
+    "_OptionalIntentConfirmationSettingOutputTypeDef",
+    {
+        "declinationResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "confirmationResponse": ResponseSpecificationOutputTypeDef,
+        "confirmationNextStep": DialogStateOutputTypeDef,
+        "confirmationConditional": ConditionalSpecificationOutputTypeDef,
+        "declinationNextStep": DialogStateOutputTypeDef,
+        "declinationConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
+    },
+    total=False,
+)
+
+
+class IntentConfirmationSettingOutputTypeDef(
+    _RequiredIntentConfirmationSettingOutputTypeDef, _OptionalIntentConfirmationSettingOutputTypeDef
+):
+    pass
+
+
+SlotCaptureSettingOutputTypeDef = TypedDict(
+    "SlotCaptureSettingOutputTypeDef",
+    {
+        "captureResponse": ResponseSpecificationOutputTypeDef,
+        "captureNextStep": DialogStateOutputTypeDef,
+        "captureConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
+    total=False,
 )
 
 InitialResponseSettingTypeDef = TypedDict(
     "InitialResponseSettingTypeDef",
     {
         "initialResponse": ResponseSpecificationTypeDef,
         "nextStep": DialogStateTypeDef,
@@ -5123,19 +6050,21 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
+
 class IntentConfirmationSettingTypeDef(
     _RequiredIntentConfirmationSettingTypeDef, _OptionalIntentConfirmationSettingTypeDef
 ):
     pass
 
+
 SlotCaptureSettingTypeDef = TypedDict(
     "SlotCaptureSettingTypeDef",
     {
         "captureResponse": ResponseSpecificationTypeDef,
         "captureNextStep": DialogStateTypeDef,
         "captureConditional": ConditionalSpecificationTypeDef,
         "failureResponse": ResponseSpecificationTypeDef,
@@ -5143,156 +6072,196 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIntentRequestRequestTypeDef",
+FulfillmentCodeHookSettingsUnionTypeDef = Union[
+    FulfillmentCodeHookSettingsTypeDef, FulfillmentCodeHookSettingsOutputTypeDef
+]
+SubSlotSettingUnionTypeDef = Union[SubSlotSettingTypeDef, SubSlotSettingOutputTypeDef]
+CreateIntentResponseTypeDef = TypedDict(
+    "CreateIntentResponseTypeDef",
     {
+        "intentId": str,
         "intentName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIntentRequestRequestTypeDef",
-    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
+        "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": Sequence[InputContextTypeDef],
-        "outputContexts": Sequence[OutputContextTypeDef],
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateIntentRequestRequestTypeDef(
-    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
-):
-    pass
-
-CreateIntentResponseTypeDef = TypedDict(
-    "CreateIntentResponseTypeDef",
+DescribeIntentResponseTypeDef = TypedDict(
+    "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "slotPriorities": List[SlotPriorityTypeDef],
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "lastUpdatedDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeIntentResponseTypeDef = TypedDict(
-    "DescribeIntentResponseTypeDef",
+UpdateIntentResponseTypeDef = TypedDict(
+    "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
         "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIntentRequestRequestTypeDef",
+_RequiredSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_RequiredSlotValueElicitationSettingOutputTypeDef",
+    {
+        "slotConstraint": SlotConstraintType,
+    },
+)
+_OptionalSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "_OptionalSlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+        "slotCaptureSetting": SlotCaptureSettingOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SlotValueElicitationSettingOutputTypeDef(
+    _RequiredSlotValueElicitationSettingOutputTypeDef,
+    _OptionalSlotValueElicitationSettingOutputTypeDef,
+):
+    pass
+
+
+InitialResponseSettingUnionTypeDef = Union[
+    InitialResponseSettingTypeDef, InitialResponseSettingOutputTypeDef
+]
+_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIntentRequestRequestTypeDef",
     {
-        "intentId": str,
         "intentName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIntentRequestRequestTypeDef",
+_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIntentRequestRequestTypeDef",
     {
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "initialResponseSetting": InitialResponseSettingTypeDef,
     },
     total=False,
 )
 
-class UpdateIntentRequestRequestTypeDef(
-    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+
+class CreateIntentRequestRequestTypeDef(
+    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
 ):
     pass
 
-UpdateIntentResponseTypeDef = TypedDict(
-    "UpdateIntentResponseTypeDef",
+
+IntentConfirmationSettingUnionTypeDef = Union[
+    IntentConfirmationSettingTypeDef, IntentConfirmationSettingOutputTypeDef
+]
+_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "intentName": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIntentRequestRequestTypeDef",
+    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
+        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "inputContexts": Sequence[InputContextTypeDef],
+        "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+
+class UpdateIntentRequestRequestTypeDef(
+    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredSlotValueElicitationSettingTypeDef = TypedDict(
     "_RequiredSlotValueElicitationSettingTypeDef",
     {
         "slotConstraint": SlotConstraintType,
     },
 )
 _OptionalSlotValueElicitationSettingTypeDef = TypedDict(
@@ -5303,130 +6272,138 @@
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "waitAndContinueSpecification": WaitAndContinueSpecificationTypeDef,
         "slotCaptureSetting": SlotCaptureSettingTypeDef,
     },
     total=False,
 )
 
+
 class SlotValueElicitationSettingTypeDef(
     _RequiredSlotValueElicitationSettingTypeDef, _OptionalSlotValueElicitationSettingTypeDef
 ):
     pass
 
-_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotRequestRequestTypeDef",
+
+CreateSlotResponseTypeDef = TypedDict(
+    "CreateSlotResponseTypeDef",
     {
+        "slotId": str,
         "slotName": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "description": str,
+        "slotTypeId": str,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-    },
-)
-_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeId": str,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "creationDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateSlotRequestRequestTypeDef(
-    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
-):
-    pass
-
-CreateSlotResponseTypeDef = TypedDict(
-    "CreateSlotResponseTypeDef",
+DescribeSlotResponseTypeDef = TypedDict(
+    "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSlotResponseTypeDef = TypedDict(
-    "DescribeSlotResponseTypeDef",
+UpdateSlotResponseTypeDef = TypedDict(
+    "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotRequestRequestTypeDef",
+_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotRequestRequestTypeDef",
     {
-        "slotId": str,
         "slotName": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
     },
 )
-_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotRequestRequestTypeDef",
+_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeId": str,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
     },
     total=False,
 )
 
-class UpdateSlotRequestRequestTypeDef(
-    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+
+class CreateSlotRequestRequestTypeDef(
+    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
 ):
     pass
 
-UpdateSlotResponseTypeDef = TypedDict(
-    "UpdateSlotResponseTypeDef",
+
+SlotValueElicitationSettingUnionTypeDef = Union[
+    SlotValueElicitationSettingTypeDef, SlotValueElicitationSettingOutputTypeDef
+]
+_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "slotName": str,
-        "description": str,
-        "slotTypeId": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeId": str,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
+
+
+class UpdateSlotRequestRequestTypeDef(
+    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/waiter.py` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models/waiter.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/PKG-INFO` & `types-aiobotocore-lexv2-models-2.5.2.post1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-lexv2-models
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexModelsV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lexv2-models type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-models"></a>
 
 # types-aiobotocore-lexv2-models
 
 [![PyPI - types-aiobotocore-lexv2-models](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lexv2-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lexv2-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-models)](https://pepy.tech/project/types-aiobotocore-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexModelsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [types-aiobotocore-lexv2-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -403,20 +370,20 @@
 )
 
 
 def check_value(value: AggregatedUtterancesFilterNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lexv2_models.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lexv2_models.type_defs import (
     ActiveContextTypeDef,
     AdvancedRecognitionSettingTypeDef,
     ExecutionErrorDetailsTypeDef,
     AgentTurnSpecificationTypeDef,
@@ -428,14 +395,15 @@
     AssociatedTranscriptTypeDef,
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
     CustomVocabularyItemTypeDef,
     FailedCustomVocabularyItemTypeDef,
+    ResponseMetadataTypeDef,
     CustomVocabularyEntryIdTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
     BotAliasTestExecutionTargetTypeDef,
     BotExportSpecificationTypeDef,
     BotFilterTypeDef,
     DataPrivacyTypeDef,
@@ -451,101 +419,86 @@
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
-    BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
     ButtonTypeDef,
     CloudWatchLogGroupLogDestinationTypeDef,
     LambdaCodeHookTypeDef,
     SubSlotTypeCompositionTypeDef,
     ConditionTypeDef,
     ConversationLevelIntentClassificationResultItemTypeDef,
     ConversationLevelResultDetailTypeDef,
     ConversationLevelSlotResolutionResultItemTypeDef,
     ConversationLevelTestResultsFilterByTypeDef,
-    ConversationLogsDataSourceFilterByTypeDef,
+    ConversationLogsDataSourceFilterByOutputTypeDef,
+    TimestampTypeDef,
     SentimentAnalysisSettingsTypeDef,
     DialogCodeHookSettingsTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     SampleUtteranceTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
-    CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
-    CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
-    CreateUploadUrlResponseTypeDef,
     CustomPayloadTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
-    DateRangeFilterTypeDef,
+    DateRangeFilterOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
-    DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
-    DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
-    DeleteBotResponseTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
-    DeleteBotVersionResponseTypeDef,
     DeleteCustomVocabularyRequestRequestTypeDef,
-    DeleteCustomVocabularyResponseTypeDef,
     DeleteExportRequestRequestTypeDef,
-    DeleteExportResponseTypeDef,
     DeleteImportRequestRequestTypeDef,
-    DeleteImportResponseTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
-    DeleteResourcePolicyStatementResponseTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
-    DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
     SlotPriorityTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
     TestSetStorageLocationTypeDef,
     DescribeTestSetRequestRequestTypeDef,
     DialogActionTypeDef,
+    IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportFilterTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
-    GetTestExecutionArtifactsUrlResponseTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
     IntentFilterTypeDef,
@@ -557,60 +510,78 @@
     RecommendedIntentSummaryTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
     PlainTextMessageTypeDef,
     SSMLMessageTypeDef,
     OverallTestResultItemTypeDef,
+    PathFormatOutputTypeDef,
     PathFormatTypeDef,
     TextInputSpecificationTypeDef,
     RelativeAggregationDurationTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     SampleValueTypeDef,
     SlotDefaultValueTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
     SlotValueTypeDef,
     SlotValueRegexFilterTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
-    StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
-    UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
-    SearchAssociatedTranscriptsResponseTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
     BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
-    ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
+    BuildBotLocaleResponseTypeDef,
+    CreateResourcePolicyResponseTypeDef,
+    CreateResourcePolicyStatementResponseTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    DeleteBotAliasResponseTypeDef,
+    DeleteBotLocaleResponseTypeDef,
+    DeleteBotResponseTypeDef,
+    DeleteBotVersionResponseTypeDef,
+    DeleteCustomVocabularyResponseTypeDef,
+    DeleteExportResponseTypeDef,
+    DeleteImportResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyStatementResponseTypeDef,
+    DescribeCustomVocabularyMetadataResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetTestExecutionArtifactsUrlResponseTypeDef,
+    ListCustomVocabularyItemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SearchAssociatedTranscriptsResponseTypeDef,
+    StopBotRecommendationResponseTypeDef,
+    UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     TestExecutionTargetTypeDef,
+    BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
     BotLocaleImportSpecificationTypeDef,
     CreateBotLocaleRequestRequestTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
     UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
@@ -629,37 +600,42 @@
     CreateBotVersionResponseTypeDef,
     ListBotVersionsRequestRequestTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsRequestRequestTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesRequestRequestTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
     TextLogDestinationTypeDef,
     CodeHookSpecificationTypeDef,
+    CompositeSlotTypeSettingOutputTypeDef,
     CompositeSlotTypeSettingTypeDef,
     ConversationLevelTestResultItemTypeDef,
     TestExecutionResultFilterByTypeDef,
-    ConversationLogsDataSourceTypeDef,
+    ConversationLogsDataSourceOutputTypeDef,
+    ConversationLogsDataSourceFilterByTypeDef,
+    DateRangeFilterTypeDef,
     IntentSummaryTypeDef,
     CreateResourcePolicyStatementRequestRequestTypeDef,
-    LexTranscriptFilterTypeDef,
+    LexTranscriptFilterOutputTypeDef,
     DescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
     DescribeBotVersionResponseTypeDef,
     UpdateBotRecommendationRequestRequestTypeDef,
     DescribeTestSetResponseTypeDef,
     TestSetSummaryTypeDef,
     UpdateTestSetResponseTypeDef,
+    DialogStateOutputTypeDef,
     DialogStateTypeDef,
     ExportResourceSpecificationTypeDef,
     ListExportsRequestRequestTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     InputSessionStateSpecificationTypeDef,
@@ -670,130 +646,178 @@
     ListSlotTypesResponseTypeDef,
     ListSlotsRequestRequestTypeDef,
     ListTestExecutionsRequestRequestTypeDef,
     ListTestSetsRequestRequestTypeDef,
     OverallTestResultsTypeDef,
     UtteranceAggregationDurationTypeDef,
     RuntimeHintDetailsTypeDef,
+    SlotTypeValueOutputTypeDef,
     SlotTypeValueTypeDef,
+    SlotDefaultValueSpecificationOutputTypeDef,
     SlotDefaultValueSpecificationTypeDef,
     SlotResolutionTestResultItemTypeDef,
+    SlotValueOverrideOutputTypeDef,
     SlotValueOverrideTypeDef,
     SlotValueSelectionSettingTypeDef,
     TestSetDiscrepancyErrorsTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
+    TestSetImportResourceSpecificationOutputTypeDef,
     TestSetImportResourceSpecificationTypeDef,
     UserTurnOutputSpecificationTypeDef,
     UtteranceInputSpecificationTypeDef,
     PromptAttemptSpecificationTypeDef,
     AudioLogSettingTypeDef,
     DescribeTestExecutionResponseTypeDef,
     StartTestExecutionRequestRequestTypeDef,
     StartTestExecutionResponseTypeDef,
     TestExecutionSummaryTypeDef,
     BotRecommendationResultsTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     TextLogSettingTypeDef,
     BotAliasLocaleSettingsTypeDef,
+    CompositeSlotTypeSettingUnionTypeDef,
     ConversationLevelTestResultsTypeDef,
     ListTestExecutionResultItemsRequestRequestTypeDef,
-    TestSetGenerationDataSourceTypeDef,
+    TestSetGenerationDataSourceOutputTypeDef,
+    ConversationLogsDataSourceTypeDef,
+    LexTranscriptFilterTypeDef,
     ListIntentsResponseTypeDef,
-    TranscriptFilterTypeDef,
+    TranscriptFilterOutputTypeDef,
     ListTestSetsResponseTypeDef,
     CreateExportRequestRequestTypeDef,
     CreateExportResponseTypeDef,
     DescribeExportResponseTypeDef,
     ExportSummaryTypeDef,
     UpdateExportResponseTypeDef,
     ExternalSourceSettingTypeDef,
     IntentClassificationTestResultsTypeDef,
     ListAggregatedUtterancesRequestRequestTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
+    SlotTypeValueUnionTypeDef,
     IntentLevelSlotResolutionTestResultItemTypeDef,
     CreateTestSetDiscrepancyReportRequestRequestTypeDef,
     CreateTestSetDiscrepancyReportResponseTypeDef,
     DescribeTestSetDiscrepancyReportResponseTypeDef,
+    ImportResourceSpecificationOutputTypeDef,
     ImportResourceSpecificationTypeDef,
     UserTurnInputSpecificationTypeDef,
     ListTestExecutionsResponseTypeDef,
+    MessageGroupOutputTypeDef,
     MessageGroupTypeDef,
+    ConversationLogSettingsOutputTypeDef,
     ConversationLogSettingsTypeDef,
     DescribeTestSetGenerationResponseTypeDef,
-    StartTestSetGenerationRequestRequestTypeDef,
     StartTestSetGenerationResponseTypeDef,
-    S3BucketTranscriptSourceTypeDef,
+    TestSetGenerationDataSourceTypeDef,
+    TranscriptFilterTypeDef,
+    S3BucketTranscriptSourceOutputTypeDef,
     ListExportsResponseTypeDef,
-    CreateSlotTypeRequestRequestTypeDef,
     CreateSlotTypeResponseTypeDef,
     DescribeSlotTypeResponseTypeDef,
-    UpdateSlotTypeRequestRequestTypeDef,
     UpdateSlotTypeResponseTypeDef,
+    CreateSlotTypeRequestRequestTypeDef,
+    UpdateSlotTypeRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultsTypeDef,
     DescribeImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    ImportResourceSpecificationUnionTypeDef,
+    StartImportRequestRequestTypeDef,
     UserTurnResultTypeDef,
     UserTurnSpecificationTypeDef,
+    FulfillmentStartResponseSpecificationOutputTypeDef,
+    FulfillmentUpdateResponseSpecificationOutputTypeDef,
+    PromptSpecificationOutputTypeDef,
+    ResponseSpecificationOutputTypeDef,
+    StillWaitingResponseSpecificationOutputTypeDef,
     FulfillmentStartResponseSpecificationTypeDef,
     FulfillmentUpdateResponseSpecificationTypeDef,
     PromptSpecificationTypeDef,
     ResponseSpecificationTypeDef,
     StillWaitingResponseSpecificationTypeDef,
-    CreateBotAliasRequestRequestTypeDef,
     CreateBotAliasResponseTypeDef,
     DescribeBotAliasResponseTypeDef,
-    UpdateBotAliasRequestRequestTypeDef,
     UpdateBotAliasResponseTypeDef,
-    TranscriptSourceSettingTypeDef,
+    ConversationLogSettingsUnionTypeDef,
+    CreateBotAliasRequestRequestTypeDef,
+    UpdateBotAliasRequestRequestTypeDef,
+    StartTestSetGenerationRequestRequestTypeDef,
+    TestSetGenerationDataSourceUnionTypeDef,
+    S3BucketTranscriptSourceTypeDef,
+    TranscriptSourceSettingOutputTypeDef,
     TestSetTurnResultTypeDef,
     TurnSpecificationTypeDef,
-    FulfillmentUpdatesSpecificationTypeDef,
+    FulfillmentUpdatesSpecificationOutputTypeDef,
     SlotSummaryTypeDef,
+    ConditionalBranchOutputTypeDef,
+    DefaultConditionalBranchOutputTypeDef,
+    WaitAndContinueSpecificationOutputTypeDef,
+    FulfillmentUpdatesSpecificationTypeDef,
     ConditionalBranchTypeDef,
     DefaultConditionalBranchTypeDef,
     WaitAndContinueSpecificationTypeDef,
+    TranscriptSourceSettingTypeDef,
     DescribeBotRecommendationResponseTypeDef,
-    StartBotRecommendationRequestRequestTypeDef,
     StartBotRecommendationResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UtteranceLevelTestResultItemTypeDef,
     TestSetTurnRecordTypeDef,
     ListSlotsResponseTypeDef,
+    ConditionalSpecificationOutputTypeDef,
+    SubSlotValueElicitationSettingOutputTypeDef,
     ConditionalSpecificationTypeDef,
     SubSlotValueElicitationSettingTypeDef,
+    StartBotRecommendationRequestRequestTypeDef,
+    TranscriptSourceSettingUnionTypeDef,
     UtteranceLevelTestResultsTypeDef,
     ListTestSetRecordsResponseTypeDef,
+    IntentClosingSettingOutputTypeDef,
+    PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    PostFulfillmentStatusSpecificationOutputTypeDef,
+    SpecificationsOutputTypeDef,
     IntentClosingSettingTypeDef,
     PostDialogCodeHookInvocationSpecificationTypeDef,
     PostFulfillmentStatusSpecificationTypeDef,
     SpecificationsTypeDef,
     TestExecutionResultItemsTypeDef,
+    DialogCodeHookInvocationSettingOutputTypeDef,
+    FulfillmentCodeHookSettingsOutputTypeDef,
+    SubSlotSettingOutputTypeDef,
+    IntentClosingSettingUnionTypeDef,
     DialogCodeHookInvocationSettingTypeDef,
     FulfillmentCodeHookSettingsTypeDef,
     SubSlotSettingTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
+    InitialResponseSettingOutputTypeDef,
+    IntentConfirmationSettingOutputTypeDef,
+    SlotCaptureSettingOutputTypeDef,
     InitialResponseSettingTypeDef,
     IntentConfirmationSettingTypeDef,
     SlotCaptureSettingTypeDef,
-    CreateIntentRequestRequestTypeDef,
+    FulfillmentCodeHookSettingsUnionTypeDef,
+    SubSlotSettingUnionTypeDef,
     CreateIntentResponseTypeDef,
     DescribeIntentResponseTypeDef,
-    UpdateIntentRequestRequestTypeDef,
     UpdateIntentResponseTypeDef,
+    SlotValueElicitationSettingOutputTypeDef,
+    InitialResponseSettingUnionTypeDef,
+    CreateIntentRequestRequestTypeDef,
+    IntentConfirmationSettingUnionTypeDef,
+    UpdateIntentRequestRequestTypeDef,
     SlotValueElicitationSettingTypeDef,
-    CreateSlotRequestRequestTypeDef,
     CreateSlotResponseTypeDef,
     DescribeSlotResponseTypeDef,
-    UpdateSlotRequestRequestTypeDef,
     UpdateSlotResponseTypeDef,
+    CreateSlotRequestRequestTypeDef,
+    SlotValueElicitationSettingUnionTypeDef,
+    UpdateSlotRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTypeDef:
+def get_value() -> ActiveContextTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt` & `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


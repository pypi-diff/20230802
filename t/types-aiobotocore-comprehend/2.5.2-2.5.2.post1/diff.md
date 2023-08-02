# Comparing `tmp/types-aiobotocore-comprehend-2.5.2.tar.gz` & `tmp/types-aiobotocore-comprehend-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehend-2.5.2.tar", last modified: Sat Jul  8 01:43:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehend-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
```

## Comparing `types-aiobotocore-comprehend-2.5.2.tar` & `types-aiobotocore-comprehend-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.197914 types-aiobotocore-comprehend-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28040 2023-07-08 01:43:26.197914 types-aiobotocore-comprehend-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26463 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:26.197914 types-aiobotocore-comprehend-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.197914 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70387 2023-07-08 01:27:52.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70284 2023-07-08 01:27:52.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-08 01:27:52.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-08 01:27:52.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-08 01:27:52.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-07-08 01:27:52.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98662 2023-07-08 01:27:55.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98585 2023-07-08 01:27:54.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:51.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.197914 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28040 2023-07-08 01:43:26.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:26.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:26.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:26.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:26.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:26.000000 types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27223 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:35:25.000000 types-aiobotocore-comprehend-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.037618 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70451 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70348 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105243 2023-08-02 14:35:29.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105154 2023-08-02 14:35:28.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehend-2.5.2/LICENSE` & `types-aiobotocore-comprehend-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2/PKG-INFO` & `types-aiobotocore-comprehend-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehend
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Comprehend 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Comprehend 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore comprehend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore comprehend type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-comprehend"></a>
 
 # types-aiobotocore-comprehend
 
 [![PyPI - types-aiobotocore-comprehend](https://img.shields.io/pypi/v/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-comprehend?color=blue)](https://pypistats.org/packages/types-aiobotocore-comprehend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehend)](https://pepy.tech/project/types-aiobotocore-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Comprehend 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [types-aiobotocore-comprehend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/).
 
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
@@ -385,60 +384,59 @@
 )
 
 
 def check_value(value: AugmentedManifestsDocumentTypeFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_comprehend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_comprehend.type_defs import (
+    AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
+    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
+    BlobTypeDef,
     ChildBlockTypeDef,
     RelationshipsListItemTypeDef,
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
     WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
+    VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
-    DatasetFilterTypeDef,
+    TimestampTypeDef,
     DatasetPropertiesTypeDef,
     DeleteDocumentClassifierRequestRequestTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEntityRecognizerRequestRequestTypeDef,
     DeleteFlywheelRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
@@ -451,98 +449,91 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
+    DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
-    DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
-    DocumentClassifierFilterTypeDef,
+    DocumentReaderConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
-    DominantLanguageDetectionJobFilterTypeDef,
-    EndpointFilterTypeDef,
-    EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
     EntityRecognizerAnnotationsTypeDef,
     EntityRecognizerDocumentsTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
-    EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
-    EventsDetectionJobFilterTypeDef,
-    FlywheelFilterTypeDef,
-    FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    ImportModelResponseTypeDef,
-    KeyPhrasesDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
-    PiiEntitiesDetectionJobFilterTypeDef,
-    SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TargetedSentimentDetectionJobFilterTypeDef,
-    TopicsDetectionJobFilterTypeDef,
-    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    RedactionConfigTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    DetectDominantLanguageResponseTypeDef,
+    ImportModelResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
@@ -552,94 +543,125 @@
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
+    DataSecurityConfigOutputTypeDef,
+    VpcConfigUnionTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
-    ListDatasetsRequestRequestTypeDef,
+    DatasetFilterTypeDef,
+    DocumentClassificationJobFilterTypeDef,
+    DocumentClassifierFilterTypeDef,
+    DominantLanguageDetectionJobFilterTypeDef,
+    EndpointFilterTypeDef,
+    EntitiesDetectionJobFilterTypeDef,
+    EntityRecognizerFilterTypeDef,
+    EventsDetectionJobFilterTypeDef,
+    FlywheelFilterTypeDef,
+    FlywheelIterationFilterTypeDef,
+    KeyPhrasesDetectionJobFilterTypeDef,
+    PiiEntitiesDetectionJobFilterTypeDef,
+    SentimentDetectionJobFilterTypeDef,
+    TargetedSentimentDetectionJobFilterTypeDef,
+    TopicsDetectionJobFilterTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigOutputTypeDef,
+    DocumentReaderConfigUnionTypeDef,
+    InputDataConfigOutputTypeDef,
+    ListDocumentClassifierSummariesResponseTypeDef,
+    DocumentMetadataTypeDef,
+    EntityRecognitionConfigOutputTypeDef,
+    EntityRecognitionConfigTypeDef,
+    EntityRecognizerInputDataConfigOutputTypeDef,
+    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerMetadataEntityTypesListItemTypeDef,
+    ListEntityRecognizerSummariesResponseTypeDef,
+    FlywheelIterationPropertiesTypeDef,
+    ListFlywheelsResponseTypeDef,
+    GeometryTypeDef,
+    SyntaxTokenTypeDef,
+    RedactionConfigUnionTypeDef,
+    BatchDetectDominantLanguageResponseTypeDef,
+    BatchDetectKeyPhrasesResponseTypeDef,
+    BatchDetectSentimentResponseTypeDef,
+    TargetedSentimentMentionTypeDef,
+    EntityTypeDef,
+    StartDocumentClassificationJobRequestRequestTypeDef,
+    StartDominantLanguageDetectionJobRequestRequestTypeDef,
+    StartEntitiesDetectionJobRequestRequestTypeDef,
+    StartEventsDetectionJobRequestRequestTypeDef,
+    StartKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StartPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StartSentimentDetectionJobRequestRequestTypeDef,
+    StartTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StartTopicsDetectionJobRequestRequestTypeDef,
+    UpdateFlywheelRequestRequestTypeDef,
+    DataSecurityConfigUnionTypeDef,
+    DatasetInputDataConfigTypeDef,
+    ListDatasetsRequestRequestTypeDef,
     ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
     ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
-    ListDocumentClassifierSummariesResponseTypeDef,
-    DocumentMetadataTypeDef,
     ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
     ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
-    EntityRecognitionConfigTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
     ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
-    EntityRecognizerMetadataEntityTypesListItemTypeDef,
-    ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
-    FlywheelIterationPropertiesTypeDef,
-    ListFlywheelsResponseTypeDef,
-    GeometryTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
-    SyntaxTokenTypeDef,
-    BatchDetectDominantLanguageResponseTypeDef,
-    BatchDetectKeyPhrasesResponseTypeDef,
-    BatchDetectSentimentResponseTypeDef,
-    TargetedSentimentMentionTypeDef,
-    EntityTypeDef,
+    CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
+    DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
-    StartDocumentClassificationJobRequestRequestTypeDef,
-    StartDominantLanguageDetectionJobRequestRequestTypeDef,
-    StartEntitiesDetectionJobRequestRequestTypeDef,
-    StartEventsDetectionJobRequestRequestTypeDef,
-    StartKeyPhrasesDetectionJobRequestRequestTypeDef,
-    StartPiiEntitiesDetectionJobRequestRequestTypeDef,
-    StartSentimentDetectionJobRequestRequestTypeDef,
-    StartTargetedSentimentDetectionJobRequestRequestTypeDef,
-    StartTopicsDetectionJobRequestRequestTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
-    UpdateFlywheelRequestRequestTypeDef,
-    DatasetInputDataConfigTypeDef,
-    CreateDocumentClassifierRequestRequestTypeDef,
-    DocumentClassifierPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
+    TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -650,34 +672,32 @@
     ListPiiEntitiesDetectionJobsResponseTypeDef,
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
-    CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
+    CreateFlywheelRequestRequestTypeDef,
+    TaskConfigUnionTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemTypeDef:
+def get_value() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-comprehend-2.5.2/README.md` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-comprehend
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Comprehend 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore comprehend type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-comprehend"></a>
 
 # types-aiobotocore-comprehend
 
 [![PyPI - types-aiobotocore-comprehend](https://img.shields.io/pypi/v/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-comprehend?color=blue)](https://pypistats.org/packages/types-aiobotocore-comprehend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehend)](https://pepy.tech/project/types-aiobotocore-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Comprehend 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [types-aiobotocore-comprehend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -352,60 +384,59 @@
 )
 
 
 def check_value(value: AugmentedManifestsDocumentTypeFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_comprehend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_comprehend.type_defs import (
+    AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
+    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
+    BlobTypeDef,
     ChildBlockTypeDef,
     RelationshipsListItemTypeDef,
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
     WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
+    VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
-    DatasetFilterTypeDef,
+    TimestampTypeDef,
     DatasetPropertiesTypeDef,
     DeleteDocumentClassifierRequestRequestTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEntityRecognizerRequestRequestTypeDef,
     DeleteFlywheelRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
@@ -418,98 +449,91 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
+    DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
-    DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
-    DocumentClassifierFilterTypeDef,
+    DocumentReaderConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
-    DominantLanguageDetectionJobFilterTypeDef,
-    EndpointFilterTypeDef,
-    EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
     EntityRecognizerAnnotationsTypeDef,
     EntityRecognizerDocumentsTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
-    EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
-    EventsDetectionJobFilterTypeDef,
-    FlywheelFilterTypeDef,
-    FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    ImportModelResponseTypeDef,
-    KeyPhrasesDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
-    PiiEntitiesDetectionJobFilterTypeDef,
-    SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TargetedSentimentDetectionJobFilterTypeDef,
-    TopicsDetectionJobFilterTypeDef,
-    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    RedactionConfigTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    DetectDominantLanguageResponseTypeDef,
+    ImportModelResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
@@ -519,94 +543,125 @@
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
+    DataSecurityConfigOutputTypeDef,
+    VpcConfigUnionTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
-    ListDatasetsRequestRequestTypeDef,
+    DatasetFilterTypeDef,
+    DocumentClassificationJobFilterTypeDef,
+    DocumentClassifierFilterTypeDef,
+    DominantLanguageDetectionJobFilterTypeDef,
+    EndpointFilterTypeDef,
+    EntitiesDetectionJobFilterTypeDef,
+    EntityRecognizerFilterTypeDef,
+    EventsDetectionJobFilterTypeDef,
+    FlywheelFilterTypeDef,
+    FlywheelIterationFilterTypeDef,
+    KeyPhrasesDetectionJobFilterTypeDef,
+    PiiEntitiesDetectionJobFilterTypeDef,
+    SentimentDetectionJobFilterTypeDef,
+    TargetedSentimentDetectionJobFilterTypeDef,
+    TopicsDetectionJobFilterTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigOutputTypeDef,
+    DocumentReaderConfigUnionTypeDef,
+    InputDataConfigOutputTypeDef,
+    ListDocumentClassifierSummariesResponseTypeDef,
+    DocumentMetadataTypeDef,
+    EntityRecognitionConfigOutputTypeDef,
+    EntityRecognitionConfigTypeDef,
+    EntityRecognizerInputDataConfigOutputTypeDef,
+    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerMetadataEntityTypesListItemTypeDef,
+    ListEntityRecognizerSummariesResponseTypeDef,
+    FlywheelIterationPropertiesTypeDef,
+    ListFlywheelsResponseTypeDef,
+    GeometryTypeDef,
+    SyntaxTokenTypeDef,
+    RedactionConfigUnionTypeDef,
+    BatchDetectDominantLanguageResponseTypeDef,
+    BatchDetectKeyPhrasesResponseTypeDef,
+    BatchDetectSentimentResponseTypeDef,
+    TargetedSentimentMentionTypeDef,
+    EntityTypeDef,
+    StartDocumentClassificationJobRequestRequestTypeDef,
+    StartDominantLanguageDetectionJobRequestRequestTypeDef,
+    StartEntitiesDetectionJobRequestRequestTypeDef,
+    StartEventsDetectionJobRequestRequestTypeDef,
+    StartKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StartPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StartSentimentDetectionJobRequestRequestTypeDef,
+    StartTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StartTopicsDetectionJobRequestRequestTypeDef,
+    UpdateFlywheelRequestRequestTypeDef,
+    DataSecurityConfigUnionTypeDef,
+    DatasetInputDataConfigTypeDef,
+    ListDatasetsRequestRequestTypeDef,
     ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
     ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
-    ListDocumentClassifierSummariesResponseTypeDef,
-    DocumentMetadataTypeDef,
     ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
     ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
-    EntityRecognitionConfigTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
     ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
-    EntityRecognizerMetadataEntityTypesListItemTypeDef,
-    ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
-    FlywheelIterationPropertiesTypeDef,
-    ListFlywheelsResponseTypeDef,
-    GeometryTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
-    SyntaxTokenTypeDef,
-    BatchDetectDominantLanguageResponseTypeDef,
-    BatchDetectKeyPhrasesResponseTypeDef,
-    BatchDetectSentimentResponseTypeDef,
-    TargetedSentimentMentionTypeDef,
-    EntityTypeDef,
+    CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
+    DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
-    StartDocumentClassificationJobRequestRequestTypeDef,
-    StartDominantLanguageDetectionJobRequestRequestTypeDef,
-    StartEntitiesDetectionJobRequestRequestTypeDef,
-    StartEventsDetectionJobRequestRequestTypeDef,
-    StartKeyPhrasesDetectionJobRequestRequestTypeDef,
-    StartPiiEntitiesDetectionJobRequestRequestTypeDef,
-    StartSentimentDetectionJobRequestRequestTypeDef,
-    StartTargetedSentimentDetectionJobRequestRequestTypeDef,
-    StartTopicsDetectionJobRequestRequestTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
-    UpdateFlywheelRequestRequestTypeDef,
-    DatasetInputDataConfigTypeDef,
-    CreateDocumentClassifierRequestRequestTypeDef,
-    DocumentClassifierPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
+    TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -617,34 +672,32 @@
     ListPiiEntitiesDetectionJobsResponseTypeDef,
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
-    CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
+    CreateFlywheelRequestRequestTypeDef,
+    TaskConfigUnionTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemTypeDef:
+def get_value() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-comprehend-2.5.2/setup.py` & `types-aiobotocore-comprehend-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehend",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Comprehend 2.5.2 service generated with"
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
-    keywords="aiobotocore comprehend type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore comprehend type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_comprehend": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/"
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/__init__.py` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/__init__.pyi` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/__main__.py` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Comprehend 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Comprehend 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/client.py` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("comprehend") as client:
         client: ComprehendClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     DatasetTypeType,
     DocumentClassifierModeType,
     LanguageCodeType,
     ModelTypeType,
@@ -44,22 +43,23 @@
 from .type_defs import (
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
+    BlobTypeDef,
     ClassifyDocumentResponseTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
-    DataSecurityConfigTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetFilterTypeDef,
     DatasetInputDataConfigTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     DescribeDocumentClassifierResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     DescribeEndpointResponseTypeDef,
@@ -79,27 +79,27 @@
     DetectKeyPhrasesResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     DetectSentimentResponseTypeDef,
     DetectSyntaxResponseTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     DocumentClassificationJobFilterTypeDef,
     DocumentClassifierFilterTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
-    DocumentReaderConfigTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityRecognizerFilterTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     ImportModelResponseTypeDef,
-    InputDataConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDatasetsResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     ListDocumentClassifiersResponseTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     ListEndpointsResponseTypeDef,
@@ -114,15 +114,15 @@
     ListSentimentDetectionJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     OutputDataConfigTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     PutResourcePolicyResponseTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigUnionTypeDef,
     SentimentDetectionJobFilterTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
@@ -135,39 +135,36 @@
     StopEventsDetectionJobResponseTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
     TagTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
-    TaskConfigTypeDef,
+    TaskConfigUnionTypeDef,
     TopicsDetectionJobFilterTypeDef,
     UpdateDataSecurityConfigTypeDef,
     UpdateEndpointResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ComprehendClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BatchSizeLimitExceededException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidFilterException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
@@ -179,15 +176,14 @@
     ResourceUnavailableException: Type[BotocoreClientError]
     TextSizeLimitExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagKeysException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     UnsupportedLanguageException: Type[BotocoreClientError]
 
-
 class ComprehendClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/)
     """
 
     meta: ClientMeta
@@ -196,123 +192,112 @@
     def exceptions(self) -> Exceptions:
         """
         ComprehendClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#exceptions)
         """
-
     async def batch_detect_dominant_language(
         self, *, TextList: Sequence[str]
     ) -> BatchDetectDominantLanguageResponseTypeDef:
         """
         Determines the dominant language of the input text for a batch of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_dominant_language)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_dominant_language)
         """
-
     async def batch_detect_entities(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectEntitiesResponseTypeDef:
         """
         Inspects the text of a batch of documents for named entities and returns
         information about them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_entities)
         """
-
     async def batch_detect_key_phrases(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectKeyPhrasesResponseTypeDef:
         """
         Detects the key noun phrases found in a batch of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_key_phrases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_key_phrases)
         """
-
     async def batch_detect_sentiment(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectSentimentResponseTypeDef:
         """
         Inspects a batch of documents and returns an inference of the prevailing
         sentiment, `POSITIVE`, `NEUTRAL`, `MIXED`, or `NEGATIVE`, in each one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_sentiment)
         """
-
     async def batch_detect_syntax(
         self, *, TextList: Sequence[str], LanguageCode: SyntaxLanguageCodeType
     ) -> BatchDetectSyntaxResponseTypeDef:
         """
         Inspects the text of a batch of documents for the syntax and part of speech of
         the words in the document and returns information about them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_syntax)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_syntax)
         """
-
     async def batch_detect_targeted_sentiment(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectTargetedSentimentResponseTypeDef:
         """
         Inspects a batch of documents and returns a sentiment analysis for each entity
         identified in the documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_targeted_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_targeted_sentiment)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#can_paginate)
         """
-
     async def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a new document classification request to analyze a single document in
         real-time, using a previously created and trained custom model and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#classify_document)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#close)
         """
-
     async def contains_pii_entities(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> ContainsPiiEntitiesResponseTypeDef:
         """
         Analyzes input text for the presence of personally identifiable information
         (PII) and returns the labels of identified PII entity types such as name,
         address, bank account number, or phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.contains_pii_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#contains_pii_entities)
         """
-
     async def create_dataset(
         self,
         *,
         FlywheelArn: str,
         DatasetName: str,
         InputDataConfig: DatasetInputDataConfigTypeDef,
         DatasetType: DatasetTypeType = ...,
@@ -323,39 +308,37 @@
         """
         Creates a dataset to upload training or test data for a model associated with a
         flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_dataset)
         """
-
     async def create_document_classifier(
         self,
         *,
         DocumentClassifierName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: DocumentClassifierInputDataConfigTypeDef,
+        InputDataConfig: DocumentClassifierInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_document_classifier)
         """
-
     async def create_endpoint(
         self,
         *,
         EndpointName: str,
         DesiredInferenceUnits: int,
         ModelArn: str = ...,
         ClientRequestToken: str = ...,
@@ -368,348 +351,316 @@
         trained custom model For information about endpoints, see [Managing
         endpoints](https://docs.aws.amazon.com/comprehend/latest/dg/manage-
         endpoints.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_endpoint)
         """
-
     async def create_entity_recognizer(
         self,
         *,
         RecognizerName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: EntityRecognizerInputDataConfigTypeDef,
+        InputDataConfig: EntityRecognizerInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_entity_recognizer)
         """
-
     async def create_flywheel(
         self,
         *,
         FlywheelName: str,
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
-        TaskConfig: TaskConfigTypeDef = ...,
+        TaskConfig: TaskConfigUnionTypeDef = ...,
         ModelType: ModelTypeType = ...,
-        DataSecurityConfig: DataSecurityConfigTypeDef = ...,
+        DataSecurityConfig: DataSecurityConfigUnionTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity recognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_flywheel)
         """
-
     async def delete_document_classifier(self, *, DocumentClassifierArn: str) -> Dict[str, Any]:
         """
         Deletes a previously created document classifier Only those classifiers that are
         in terminated states (IN_ERROR, TRAINED) will be deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_document_classifier)
         """
-
     async def delete_endpoint(self, *, EndpointArn: str) -> Dict[str, Any]:
         """
         Deletes a model-specific endpoint for a previously-trained custom model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_endpoint)
         """
-
     async def delete_entity_recognizer(self, *, EntityRecognizerArn: str) -> Dict[str, Any]:
         """
         Deletes an entity recognizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_entity_recognizer)
         """
-
     async def delete_flywheel(self, *, FlywheelArn: str) -> Dict[str, Any]:
         """
         Deletes a flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_flywheel)
         """
-
     async def delete_resource_policy(
         self, *, ResourceArn: str, PolicyRevisionId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a resource-based policy that is attached to a custom model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_resource_policy)
         """
-
     async def describe_dataset(self, *, DatasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Returns information about the dataset that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_dataset)
         """
-
     async def describe_document_classification_job(
         self, *, JobId: str
     ) -> DescribeDocumentClassificationJobResponseTypeDef:
         """
         Gets the properties associated with a document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_document_classification_job)
         """
-
     async def describe_document_classifier(
         self, *, DocumentClassifierArn: str
     ) -> DescribeDocumentClassifierResponseTypeDef:
         """
         Gets the properties associated with a document classifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_document_classifier)
         """
-
     async def describe_dominant_language_detection_job(
         self, *, JobId: str
     ) -> DescribeDominantLanguageDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a dominant language detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_dominant_language_detection_job)
         """
-
     async def describe_endpoint(self, *, EndpointArn: str) -> DescribeEndpointResponseTypeDef:
         """
         Gets the properties associated with a specific endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_endpoint)
         """
-
     async def describe_entities_detection_job(
         self, *, JobId: str
     ) -> DescribeEntitiesDetectionJobResponseTypeDef:
         """
         Gets the properties associated with an entities detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_entities_detection_job)
         """
-
     async def describe_entity_recognizer(
         self, *, EntityRecognizerArn: str
     ) -> DescribeEntityRecognizerResponseTypeDef:
         """
         Provides details about an entity recognizer including status, S3 buckets
         containing training data, recognizer metadata, metrics, and so on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_entity_recognizer)
         """
-
     async def describe_events_detection_job(
         self, *, JobId: str
     ) -> DescribeEventsDetectionJobResponseTypeDef:
         """
         Gets the status and details of an events detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_events_detection_job)
         """
-
     async def describe_flywheel(self, *, FlywheelArn: str) -> DescribeFlywheelResponseTypeDef:
         """
         Provides configuration information about the flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_flywheel)
         """
-
     async def describe_flywheel_iteration(
         self, *, FlywheelArn: str, FlywheelIterationId: str
     ) -> DescribeFlywheelIterationResponseTypeDef:
         """
         Retrieve the configuration properties of a flywheel iteration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_flywheel_iteration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_flywheel_iteration)
         """
-
     async def describe_key_phrases_detection_job(
         self, *, JobId: str
     ) -> DescribeKeyPhrasesDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a key phrases detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_key_phrases_detection_job)
         """
-
     async def describe_pii_entities_detection_job(
         self, *, JobId: str
     ) -> DescribePiiEntitiesDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a PII entities detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_pii_entities_detection_job)
         """
-
     async def describe_resource_policy(
         self, *, ResourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Gets the details of a resource-based policy that is attached to a custom model,
         including the JSON body of the policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_resource_policy)
         """
-
     async def describe_sentiment_detection_job(
         self, *, JobId: str
     ) -> DescribeSentimentDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a sentiment detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_sentiment_detection_job)
         """
-
     async def describe_targeted_sentiment_detection_job(
         self, *, JobId: str
     ) -> DescribeTargetedSentimentDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a targeted sentiment detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_targeted_sentiment_detection_job)
         """
-
     async def describe_topics_detection_job(
         self, *, JobId: str
     ) -> DescribeTopicsDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_topics_detection_job)
         """
-
     async def detect_dominant_language(self, *, Text: str) -> DetectDominantLanguageResponseTypeDef:
         """
         Determines the dominant language of the input text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_dominant_language)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_dominant_language)
         """
-
     async def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_entities)
         """
-
     async def detect_key_phrases(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectKeyPhrasesResponseTypeDef:
         """
         Detects the key noun phrases found in the text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_key_phrases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_key_phrases)
         """
-
     async def detect_pii_entities(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectPiiEntitiesResponseTypeDef:
         """
         Inspects the input text for entities that contain personally identifiable
         information (PII) and returns information about them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_pii_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_pii_entities)
         """
-
     async def detect_sentiment(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectSentimentResponseTypeDef:
         """
         Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`,
         `NEUTRAL`, `MIXED`, or `NEGATIVE`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_sentiment)
         """
-
     async def detect_syntax(
         self, *, Text: str, LanguageCode: SyntaxLanguageCodeType
     ) -> DetectSyntaxResponseTypeDef:
         """
         Inspects text for syntax and the part of speech of words in the document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_syntax)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_syntax)
         """
-
     async def detect_targeted_sentiment(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectTargetedSentimentResponseTypeDef:
         """
         Inspects the input text and returns a sentiment analysis for each entity
         identified in the text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_targeted_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_targeted_sentiment)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#generate_presigned_url)
         """
-
     async def import_model(
         self,
         *,
         SourceModelArn: str,
         ModelName: str = ...,
         VersionName: str = ...,
         ModelKmsKeyId: str = ...,
@@ -719,560 +670,519 @@
         """
         Creates a new custom model that replicates a source custom model that you
         import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.import_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#import_model)
         """
-
     async def list_datasets(
         self,
         *,
         FlywheelArn: str = ...,
         Filter: DatasetFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDatasetsResponseTypeDef:
         """
         List the datasets that you have configured in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_datasets)
         """
-
     async def list_document_classification_jobs(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDocumentClassificationJobsResponseTypeDef:
         """
         Gets a list of the documentation classification jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classification_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classification_jobs)
         """
-
     async def list_document_classifier_summaries(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDocumentClassifierSummariesResponseTypeDef:
         """
         Gets a list of summaries of the document classifiers that you have created See
         also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/comprehend-2017-11-27/ListDocumentClassifierSummaries).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifier_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classifier_summaries)
         """
-
     async def list_document_classifiers(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDocumentClassifiersResponseTypeDef:
         """
         Gets a list of the document classifiers that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classifiers)
         """
-
     async def list_dominant_language_detection_jobs(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDominantLanguageDetectionJobsResponseTypeDef:
         """
         Gets a list of the dominant language detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_dominant_language_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_dominant_language_detection_jobs)
         """
-
     async def list_endpoints(
         self, *, Filter: EndpointFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListEndpointsResponseTypeDef:
         """
         Gets a list of all existing endpoints that you've created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_endpoints)
         """
-
     async def list_entities_detection_jobs(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entities_detection_jobs)
         """
-
     async def list_entity_recognizer_summaries(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEntityRecognizerSummariesResponseTypeDef:
         """
         Gets a list of summaries for the entity recognizers that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizer_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entity_recognizer_summaries)
         """
-
     async def list_entity_recognizers(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListEntityRecognizersResponseTypeDef:
         """
         Gets a list of the properties of all entity recognizers that you created,
         including recognizers currently in training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entity_recognizers)
         """
-
     async def list_events_detection_jobs(
         self,
         *,
         Filter: EventsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListEventsDetectionJobsResponseTypeDef:
         """
         Gets a list of the events detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_events_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_events_detection_jobs)
         """
-
     async def list_flywheel_iteration_history(
         self,
         *,
         FlywheelArn: str,
         Filter: FlywheelIterationFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListFlywheelIterationHistoryResponseTypeDef:
         """
         Information about the history of a flywheel iteration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheel_iteration_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_flywheel_iteration_history)
         """
-
     async def list_flywheels(
         self, *, Filter: FlywheelFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListFlywheelsResponseTypeDef:
         """
         Gets a list of the flywheels that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_flywheels)
         """
-
     async def list_key_phrases_detection_jobs(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListKeyPhrasesDetectionJobsResponseTypeDef:
         """
         Get a list of key phrase detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_key_phrases_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_key_phrases_detection_jobs)
         """
-
     async def list_pii_entities_detection_jobs(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPiiEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the PII entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_pii_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_pii_entities_detection_jobs)
         """
-
     async def list_sentiment_detection_jobs(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_sentiment_detection_jobs)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags associated with a given Amazon Comprehend resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_tags_for_resource)
         """
-
     async def list_targeted_sentiment_detection_jobs(
         self,
         *,
         Filter: TargetedSentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTargetedSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of targeted sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_targeted_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_targeted_sentiment_detection_jobs)
         """
-
     async def list_topics_detection_jobs(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTopicsDetectionJobsResponseTypeDef:
         """
         Gets a list of the topic detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_topics_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_topics_detection_jobs)
         """
-
     async def put_resource_policy(
         self, *, ResourceArn: str, ResourcePolicy: str, PolicyRevisionId: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Attaches a resource-based policy to a custom model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#put_resource_policy)
         """
-
     async def start_document_classification_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_document_classification_job)
         """
-
     async def start_dominant_language_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_dominant_language_detection_job)
         """
-
     async def start_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_entities_detection_job)
         """
-
     async def start_events_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartEventsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous event detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_events_detection_job)
         """
-
     async def start_flywheel_iteration(
         self, *, FlywheelArn: str, ClientRequestToken: str = ...
     ) -> StartFlywheelIterationResponseTypeDef:
         """
         Start the flywheel iteration.This operation uses any new datasets to train a new
         model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_flywheel_iteration)
         """
-
     async def start_key_phrases_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_key_phrases_detection_job)
         """
-
     async def start_pii_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
-        RedactionConfig: RedactionConfigTypeDef = ...,
+        RedactionConfig: RedactionConfigUnionTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_pii_entities_detection_job)
         """
-
     async def start_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_sentiment_detection_job)
         """
-
     async def start_targeted_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_targeted_sentiment_detection_job)
         """
-
     async def start_topics_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_topics_detection_job)
         """
-
     async def stop_dominant_language_detection_job(
         self, *, JobId: str
     ) -> StopDominantLanguageDetectionJobResponseTypeDef:
         """
         Stops a dominant language detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_dominant_language_detection_job)
         """
-
     async def stop_entities_detection_job(
         self, *, JobId: str
     ) -> StopEntitiesDetectionJobResponseTypeDef:
         """
         Stops an entities detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_entities_detection_job)
         """
-
     async def stop_events_detection_job(
         self, *, JobId: str
     ) -> StopEventsDetectionJobResponseTypeDef:
         """
         Stops an events detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_events_detection_job)
         """
-
     async def stop_key_phrases_detection_job(
         self, *, JobId: str
     ) -> StopKeyPhrasesDetectionJobResponseTypeDef:
         """
         Stops a key phrases detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_key_phrases_detection_job)
         """
-
     async def stop_pii_entities_detection_job(
         self, *, JobId: str
     ) -> StopPiiEntitiesDetectionJobResponseTypeDef:
         """
         Stops a PII entities detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_pii_entities_detection_job)
         """
-
     async def stop_sentiment_detection_job(
         self, *, JobId: str
     ) -> StopSentimentDetectionJobResponseTypeDef:
         """
         Stops a sentiment detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_sentiment_detection_job)
         """
-
     async def stop_targeted_sentiment_detection_job(
         self, *, JobId: str
     ) -> StopTargetedSentimentDetectionJobResponseTypeDef:
         """
         Stops a targeted sentiment detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_targeted_sentiment_detection_job)
         """
-
     async def stop_training_document_classifier(
         self, *, DocumentClassifierArn: str
     ) -> Dict[str, Any]:
         """
         Stops a document classifier training job while in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_training_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_training_document_classifier)
         """
-
     async def stop_training_entity_recognizer(self, *, EntityRecognizerArn: str) -> Dict[str, Any]:
         """
         Stops an entity recognizer training job while in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_training_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_training_entity_recognizer)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Associates a specific tag with an Amazon Comprehend resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a specific tag associated with an Amazon Comprehend resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#untag_resource)
         """
-
     async def update_endpoint(
         self,
         *,
         EndpointArn: str,
         DesiredModelArn: str = ...,
         DesiredInferenceUnits: int = ...,
         DesiredDataAccessRoleArn: str = ...,
@@ -1280,122 +1190,109 @@
     ) -> UpdateEndpointResponseTypeDef:
         """
         Updates information about the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_endpoint)
         """
-
     async def update_flywheel(
         self,
         *,
         FlywheelArn: str,
         ActiveModelArn: str = ...,
         DataAccessRoleArn: str = ...,
         DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...
     ) -> UpdateFlywheelResponseTypeDef:
         """
         Update the configuration information for an existing flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_flywheel)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_classification_jobs"]
     ) -> ListDocumentClassificationJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_classifiers"]
     ) -> ListDocumentClassifiersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dominant_language_detection_jobs"]
     ) -> ListDominantLanguageDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_endpoints"]) -> ListEndpointsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_entities_detection_jobs"]
     ) -> ListEntitiesDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_entity_recognizers"]
     ) -> ListEntityRecognizersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_key_phrases_detection_jobs"]
     ) -> ListKeyPhrasesDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_pii_entities_detection_jobs"]
     ) -> ListPiiEntitiesDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_sentiment_detection_jobs"]
     ) -> ListSentimentDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_topics_detection_jobs"]
     ) -> ListTopicsDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "ComprehendClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/)
         """
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/client.pyi` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("comprehend") as client:
         client: ComprehendClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     DatasetTypeType,
     DocumentClassifierModeType,
     LanguageCodeType,
     ModelTypeType,
@@ -44,22 +43,23 @@
 from .type_defs import (
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
+    BlobTypeDef,
     ClassifyDocumentResponseTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
-    DataSecurityConfigTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetFilterTypeDef,
     DatasetInputDataConfigTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     DescribeDocumentClassifierResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     DescribeEndpointResponseTypeDef,
@@ -79,27 +79,27 @@
     DetectKeyPhrasesResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     DetectSentimentResponseTypeDef,
     DetectSyntaxResponseTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     DocumentClassificationJobFilterTypeDef,
     DocumentClassifierFilterTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
-    DocumentReaderConfigTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityRecognizerFilterTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     ImportModelResponseTypeDef,
-    InputDataConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDatasetsResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     ListDocumentClassifiersResponseTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     ListEndpointsResponseTypeDef,
@@ -114,15 +114,15 @@
     ListSentimentDetectionJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     OutputDataConfigTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     PutResourcePolicyResponseTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigUnionTypeDef,
     SentimentDetectionJobFilterTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
@@ -135,36 +135,39 @@
     StopEventsDetectionJobResponseTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
     TagTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
-    TaskConfigTypeDef,
+    TaskConfigUnionTypeDef,
     TopicsDetectionJobFilterTypeDef,
     UpdateDataSecurityConfigTypeDef,
     UpdateEndpointResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ComprehendClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BatchSizeLimitExceededException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidFilterException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
@@ -176,14 +179,15 @@
     ResourceUnavailableException: Type[BotocoreClientError]
     TextSizeLimitExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagKeysException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     UnsupportedLanguageException: Type[BotocoreClientError]
 
+
 class ComprehendClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/)
     """
 
     meta: ClientMeta
@@ -192,112 +196,123 @@
     def exceptions(self) -> Exceptions:
         """
         ComprehendClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#exceptions)
         """
+
     async def batch_detect_dominant_language(
         self, *, TextList: Sequence[str]
     ) -> BatchDetectDominantLanguageResponseTypeDef:
         """
         Determines the dominant language of the input text for a batch of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_dominant_language)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_dominant_language)
         """
+
     async def batch_detect_entities(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectEntitiesResponseTypeDef:
         """
         Inspects the text of a batch of documents for named entities and returns
         information about them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_entities)
         """
+
     async def batch_detect_key_phrases(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectKeyPhrasesResponseTypeDef:
         """
         Detects the key noun phrases found in a batch of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_key_phrases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_key_phrases)
         """
+
     async def batch_detect_sentiment(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectSentimentResponseTypeDef:
         """
         Inspects a batch of documents and returns an inference of the prevailing
         sentiment, `POSITIVE`, `NEUTRAL`, `MIXED`, or `NEGATIVE`, in each one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_sentiment)
         """
+
     async def batch_detect_syntax(
         self, *, TextList: Sequence[str], LanguageCode: SyntaxLanguageCodeType
     ) -> BatchDetectSyntaxResponseTypeDef:
         """
         Inspects the text of a batch of documents for the syntax and part of speech of
         the words in the document and returns information about them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_syntax)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_syntax)
         """
+
     async def batch_detect_targeted_sentiment(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectTargetedSentimentResponseTypeDef:
         """
         Inspects a batch of documents and returns a sentiment analysis for each entity
         identified in the documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_targeted_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#batch_detect_targeted_sentiment)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#can_paginate)
         """
+
     async def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a new document classification request to analyze a single document in
         real-time, using a previously created and trained custom model and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#classify_document)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#close)
         """
+
     async def contains_pii_entities(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> ContainsPiiEntitiesResponseTypeDef:
         """
         Analyzes input text for the presence of personally identifiable information
         (PII) and returns the labels of identified PII entity types such as name,
         address, bank account number, or phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.contains_pii_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#contains_pii_entities)
         """
+
     async def create_dataset(
         self,
         *,
         FlywheelArn: str,
         DatasetName: str,
         InputDataConfig: DatasetInputDataConfigTypeDef,
         DatasetType: DatasetTypeType = ...,
@@ -308,37 +323,39 @@
         """
         Creates a dataset to upload training or test data for a model associated with a
         flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_dataset)
         """
+
     async def create_document_classifier(
         self,
         *,
         DocumentClassifierName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: DocumentClassifierInputDataConfigTypeDef,
+        InputDataConfig: DocumentClassifierInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_document_classifier)
         """
+
     async def create_endpoint(
         self,
         *,
         EndpointName: str,
         DesiredInferenceUnits: int,
         ModelArn: str = ...,
         ClientRequestToken: str = ...,
@@ -351,316 +368,348 @@
         trained custom model For information about endpoints, see [Managing
         endpoints](https://docs.aws.amazon.com/comprehend/latest/dg/manage-
         endpoints.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_endpoint)
         """
+
     async def create_entity_recognizer(
         self,
         *,
         RecognizerName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: EntityRecognizerInputDataConfigTypeDef,
+        InputDataConfig: EntityRecognizerInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_entity_recognizer)
         """
+
     async def create_flywheel(
         self,
         *,
         FlywheelName: str,
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
-        TaskConfig: TaskConfigTypeDef = ...,
+        TaskConfig: TaskConfigUnionTypeDef = ...,
         ModelType: ModelTypeType = ...,
-        DataSecurityConfig: DataSecurityConfigTypeDef = ...,
+        DataSecurityConfig: DataSecurityConfigUnionTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity recognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_flywheel)
         """
+
     async def delete_document_classifier(self, *, DocumentClassifierArn: str) -> Dict[str, Any]:
         """
         Deletes a previously created document classifier Only those classifiers that are
         in terminated states (IN_ERROR, TRAINED) will be deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_document_classifier)
         """
+
     async def delete_endpoint(self, *, EndpointArn: str) -> Dict[str, Any]:
         """
         Deletes a model-specific endpoint for a previously-trained custom model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_endpoint)
         """
+
     async def delete_entity_recognizer(self, *, EntityRecognizerArn: str) -> Dict[str, Any]:
         """
         Deletes an entity recognizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_entity_recognizer)
         """
+
     async def delete_flywheel(self, *, FlywheelArn: str) -> Dict[str, Any]:
         """
         Deletes a flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_flywheel)
         """
+
     async def delete_resource_policy(
         self, *, ResourceArn: str, PolicyRevisionId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a resource-based policy that is attached to a custom model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#delete_resource_policy)
         """
+
     async def describe_dataset(self, *, DatasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Returns information about the dataset that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_dataset)
         """
+
     async def describe_document_classification_job(
         self, *, JobId: str
     ) -> DescribeDocumentClassificationJobResponseTypeDef:
         """
         Gets the properties associated with a document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_document_classification_job)
         """
+
     async def describe_document_classifier(
         self, *, DocumentClassifierArn: str
     ) -> DescribeDocumentClassifierResponseTypeDef:
         """
         Gets the properties associated with a document classifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_document_classifier)
         """
+
     async def describe_dominant_language_detection_job(
         self, *, JobId: str
     ) -> DescribeDominantLanguageDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a dominant language detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_dominant_language_detection_job)
         """
+
     async def describe_endpoint(self, *, EndpointArn: str) -> DescribeEndpointResponseTypeDef:
         """
         Gets the properties associated with a specific endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_endpoint)
         """
+
     async def describe_entities_detection_job(
         self, *, JobId: str
     ) -> DescribeEntitiesDetectionJobResponseTypeDef:
         """
         Gets the properties associated with an entities detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_entities_detection_job)
         """
+
     async def describe_entity_recognizer(
         self, *, EntityRecognizerArn: str
     ) -> DescribeEntityRecognizerResponseTypeDef:
         """
         Provides details about an entity recognizer including status, S3 buckets
         containing training data, recognizer metadata, metrics, and so on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_entity_recognizer)
         """
+
     async def describe_events_detection_job(
         self, *, JobId: str
     ) -> DescribeEventsDetectionJobResponseTypeDef:
         """
         Gets the status and details of an events detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_events_detection_job)
         """
+
     async def describe_flywheel(self, *, FlywheelArn: str) -> DescribeFlywheelResponseTypeDef:
         """
         Provides configuration information about the flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_flywheel)
         """
+
     async def describe_flywheel_iteration(
         self, *, FlywheelArn: str, FlywheelIterationId: str
     ) -> DescribeFlywheelIterationResponseTypeDef:
         """
         Retrieve the configuration properties of a flywheel iteration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_flywheel_iteration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_flywheel_iteration)
         """
+
     async def describe_key_phrases_detection_job(
         self, *, JobId: str
     ) -> DescribeKeyPhrasesDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a key phrases detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_key_phrases_detection_job)
         """
+
     async def describe_pii_entities_detection_job(
         self, *, JobId: str
     ) -> DescribePiiEntitiesDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a PII entities detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_pii_entities_detection_job)
         """
+
     async def describe_resource_policy(
         self, *, ResourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Gets the details of a resource-based policy that is attached to a custom model,
         including the JSON body of the policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_resource_policy)
         """
+
     async def describe_sentiment_detection_job(
         self, *, JobId: str
     ) -> DescribeSentimentDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a sentiment detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_sentiment_detection_job)
         """
+
     async def describe_targeted_sentiment_detection_job(
         self, *, JobId: str
     ) -> DescribeTargetedSentimentDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a targeted sentiment detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_targeted_sentiment_detection_job)
         """
+
     async def describe_topics_detection_job(
         self, *, JobId: str
     ) -> DescribeTopicsDetectionJobResponseTypeDef:
         """
         Gets the properties associated with a topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#describe_topics_detection_job)
         """
+
     async def detect_dominant_language(self, *, Text: str) -> DetectDominantLanguageResponseTypeDef:
         """
         Determines the dominant language of the input text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_dominant_language)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_dominant_language)
         """
+
     async def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_entities)
         """
+
     async def detect_key_phrases(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectKeyPhrasesResponseTypeDef:
         """
         Detects the key noun phrases found in the text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_key_phrases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_key_phrases)
         """
+
     async def detect_pii_entities(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectPiiEntitiesResponseTypeDef:
         """
         Inspects the input text for entities that contain personally identifiable
         information (PII) and returns information about them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_pii_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_pii_entities)
         """
+
     async def detect_sentiment(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectSentimentResponseTypeDef:
         """
         Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`,
         `NEUTRAL`, `MIXED`, or `NEGATIVE`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_sentiment)
         """
+
     async def detect_syntax(
         self, *, Text: str, LanguageCode: SyntaxLanguageCodeType
     ) -> DetectSyntaxResponseTypeDef:
         """
         Inspects text for syntax and the part of speech of words in the document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_syntax)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_syntax)
         """
+
     async def detect_targeted_sentiment(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectTargetedSentimentResponseTypeDef:
         """
         Inspects the input text and returns a sentiment analysis for each entity
         identified in the text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_targeted_sentiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_targeted_sentiment)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#generate_presigned_url)
         """
+
     async def import_model(
         self,
         *,
         SourceModelArn: str,
         ModelName: str = ...,
         VersionName: str = ...,
         ModelKmsKeyId: str = ...,
@@ -670,519 +719,560 @@
         """
         Creates a new custom model that replicates a source custom model that you
         import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.import_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#import_model)
         """
+
     async def list_datasets(
         self,
         *,
         FlywheelArn: str = ...,
         Filter: DatasetFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDatasetsResponseTypeDef:
         """
         List the datasets that you have configured in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_datasets)
         """
+
     async def list_document_classification_jobs(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDocumentClassificationJobsResponseTypeDef:
         """
         Gets a list of the documentation classification jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classification_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classification_jobs)
         """
+
     async def list_document_classifier_summaries(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDocumentClassifierSummariesResponseTypeDef:
         """
         Gets a list of summaries of the document classifiers that you have created See
         also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/comprehend-2017-11-27/ListDocumentClassifierSummaries).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifier_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classifier_summaries)
         """
+
     async def list_document_classifiers(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDocumentClassifiersResponseTypeDef:
         """
         Gets a list of the document classifiers that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classifiers)
         """
+
     async def list_dominant_language_detection_jobs(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDominantLanguageDetectionJobsResponseTypeDef:
         """
         Gets a list of the dominant language detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_dominant_language_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_dominant_language_detection_jobs)
         """
+
     async def list_endpoints(
         self, *, Filter: EndpointFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListEndpointsResponseTypeDef:
         """
         Gets a list of all existing endpoints that you've created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_endpoints)
         """
+
     async def list_entities_detection_jobs(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entities_detection_jobs)
         """
+
     async def list_entity_recognizer_summaries(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEntityRecognizerSummariesResponseTypeDef:
         """
         Gets a list of summaries for the entity recognizers that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizer_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entity_recognizer_summaries)
         """
+
     async def list_entity_recognizers(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListEntityRecognizersResponseTypeDef:
         """
         Gets a list of the properties of all entity recognizers that you created,
         including recognizers currently in training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entity_recognizers)
         """
+
     async def list_events_detection_jobs(
         self,
         *,
         Filter: EventsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListEventsDetectionJobsResponseTypeDef:
         """
         Gets a list of the events detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_events_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_events_detection_jobs)
         """
+
     async def list_flywheel_iteration_history(
         self,
         *,
         FlywheelArn: str,
         Filter: FlywheelIterationFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListFlywheelIterationHistoryResponseTypeDef:
         """
         Information about the history of a flywheel iteration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheel_iteration_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_flywheel_iteration_history)
         """
+
     async def list_flywheels(
         self, *, Filter: FlywheelFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListFlywheelsResponseTypeDef:
         """
         Gets a list of the flywheels that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_flywheels)
         """
+
     async def list_key_phrases_detection_jobs(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListKeyPhrasesDetectionJobsResponseTypeDef:
         """
         Get a list of key phrase detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_key_phrases_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_key_phrases_detection_jobs)
         """
+
     async def list_pii_entities_detection_jobs(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPiiEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the PII entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_pii_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_pii_entities_detection_jobs)
         """
+
     async def list_sentiment_detection_jobs(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_sentiment_detection_jobs)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags associated with a given Amazon Comprehend resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_tags_for_resource)
         """
+
     async def list_targeted_sentiment_detection_jobs(
         self,
         *,
         Filter: TargetedSentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTargetedSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of targeted sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_targeted_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_targeted_sentiment_detection_jobs)
         """
+
     async def list_topics_detection_jobs(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTopicsDetectionJobsResponseTypeDef:
         """
         Gets a list of the topic detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_topics_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_topics_detection_jobs)
         """
+
     async def put_resource_policy(
         self, *, ResourceArn: str, ResourcePolicy: str, PolicyRevisionId: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Attaches a resource-based policy to a custom model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#put_resource_policy)
         """
+
     async def start_document_classification_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_document_classification_job)
         """
+
     async def start_dominant_language_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_dominant_language_detection_job)
         """
+
     async def start_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_entities_detection_job)
         """
+
     async def start_events_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartEventsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous event detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_events_detection_job)
         """
+
     async def start_flywheel_iteration(
         self, *, FlywheelArn: str, ClientRequestToken: str = ...
     ) -> StartFlywheelIterationResponseTypeDef:
         """
         Start the flywheel iteration.This operation uses any new datasets to train a new
         model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_flywheel_iteration)
         """
+
     async def start_key_phrases_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_key_phrases_detection_job)
         """
+
     async def start_pii_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
-        RedactionConfig: RedactionConfigTypeDef = ...,
+        RedactionConfig: RedactionConfigUnionTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_pii_entities_detection_job)
         """
+
     async def start_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_sentiment_detection_job)
         """
+
     async def start_targeted_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_targeted_sentiment_detection_job)
         """
+
     async def start_topics_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_topics_detection_job)
         """
+
     async def stop_dominant_language_detection_job(
         self, *, JobId: str
     ) -> StopDominantLanguageDetectionJobResponseTypeDef:
         """
         Stops a dominant language detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_dominant_language_detection_job)
         """
+
     async def stop_entities_detection_job(
         self, *, JobId: str
     ) -> StopEntitiesDetectionJobResponseTypeDef:
         """
         Stops an entities detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_entities_detection_job)
         """
+
     async def stop_events_detection_job(
         self, *, JobId: str
     ) -> StopEventsDetectionJobResponseTypeDef:
         """
         Stops an events detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_events_detection_job)
         """
+
     async def stop_key_phrases_detection_job(
         self, *, JobId: str
     ) -> StopKeyPhrasesDetectionJobResponseTypeDef:
         """
         Stops a key phrases detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_key_phrases_detection_job)
         """
+
     async def stop_pii_entities_detection_job(
         self, *, JobId: str
     ) -> StopPiiEntitiesDetectionJobResponseTypeDef:
         """
         Stops a PII entities detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_pii_entities_detection_job)
         """
+
     async def stop_sentiment_detection_job(
         self, *, JobId: str
     ) -> StopSentimentDetectionJobResponseTypeDef:
         """
         Stops a sentiment detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_sentiment_detection_job)
         """
+
     async def stop_targeted_sentiment_detection_job(
         self, *, JobId: str
     ) -> StopTargetedSentimentDetectionJobResponseTypeDef:
         """
         Stops a targeted sentiment detection job in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_targeted_sentiment_detection_job)
         """
+
     async def stop_training_document_classifier(
         self, *, DocumentClassifierArn: str
     ) -> Dict[str, Any]:
         """
         Stops a document classifier training job while in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_training_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_training_document_classifier)
         """
+
     async def stop_training_entity_recognizer(self, *, EntityRecognizerArn: str) -> Dict[str, Any]:
         """
         Stops an entity recognizer training job while in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_training_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#stop_training_entity_recognizer)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Associates a specific tag with an Amazon Comprehend resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a specific tag associated with an Amazon Comprehend resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#untag_resource)
         """
+
     async def update_endpoint(
         self,
         *,
         EndpointArn: str,
         DesiredModelArn: str = ...,
         DesiredInferenceUnits: int = ...,
         DesiredDataAccessRoleArn: str = ...,
@@ -1190,109 +1280,122 @@
     ) -> UpdateEndpointResponseTypeDef:
         """
         Updates information about the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_endpoint)
         """
+
     async def update_flywheel(
         self,
         *,
         FlywheelArn: str,
         ActiveModelArn: str = ...,
         DataAccessRoleArn: str = ...,
         DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...
     ) -> UpdateFlywheelResponseTypeDef:
         """
         Update the configuration information for an existing flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_flywheel)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_classification_jobs"]
     ) -> ListDocumentClassificationJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_classifiers"]
     ) -> ListDocumentClassifiersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dominant_language_detection_jobs"]
     ) -> ListDominantLanguageDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_endpoints"]) -> ListEndpointsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_entities_detection_jobs"]
     ) -> ListEntitiesDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_entity_recognizers"]
     ) -> ListEntityRecognizersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_key_phrases_detection_jobs"]
     ) -> ListKeyPhrasesDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_pii_entities_detection_jobs"]
     ) -> ListPiiEntitiesDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_sentiment_detection_jobs"]
     ) -> ListSentimentDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_topics_detection_jobs"]
     ) -> ListTopicsDetectionJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "ComprehendClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/)
         """
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/literals.py` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/literals.pyi` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/paginator.py` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 
@@ -115,15 +115,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 
@@ -133,33 +133,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 
 class ListEndpointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Filter: EndpointFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: EndpointFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listendpointspaginator)
         """
 
 
@@ -169,15 +166,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 
@@ -187,15 +184,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntityRecognizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 
@@ -205,15 +202,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 
@@ -223,15 +220,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 
@@ -241,15 +238,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSentimentDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 
@@ -259,13 +256,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTopicsDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/paginator.pyi` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 class ListDocumentClassifiersPaginator(AioPaginator):
@@ -111,15 +111,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 class ListDominantLanguageDetectionJobsPaginator(AioPaginator):
@@ -128,32 +128,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 class ListEndpointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Filter: EndpointFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: EndpointFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listendpointspaginator)
         """
 
 class ListEntitiesDetectionJobsPaginator(AioPaginator):
@@ -162,15 +159,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 class ListEntityRecognizersPaginator(AioPaginator):
@@ -179,15 +176,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntityRecognizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 class ListKeyPhrasesDetectionJobsPaginator(AioPaginator):
@@ -196,15 +193,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 class ListPiiEntitiesDetectionJobsPaginator(AioPaginator):
@@ -213,15 +210,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 class ListSentimentDetectionJobsPaginator(AioPaginator):
@@ -230,15 +227,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSentimentDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 class ListTopicsDetectionJobsPaginator(AioPaginator):
@@ -247,13 +244,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTopicsDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/type_defs.py` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for comprehend service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemTypeDef
+    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
 
-    data: AugmentedManifestsListItemTypeDef = {...}
+    data: AugmentedManifestsListItemOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -59,51 +59,50 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
+    "BlobTypeDef",
     "ChildBlockTypeDef",
     "RelationshipsListItemTypeDef",
     "BoundingBoxTypeDef",
     "ClassifierEvaluationMetricsTypeDef",
     "DocumentReaderConfigTypeDef",
     "DocumentClassTypeDef",
     "DocumentLabelTypeDef",
     "DocumentTypeListItemTypeDef",
     "ErrorsListItemTypeDef",
     "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
-    "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
-    "CreateDocumentClassifierResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreateEntityRecognizerResponseTypeDef",
-    "CreateFlywheelResponseTypeDef",
+    "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
-    "DatasetFilterTypeDef",
+    "TimestampTypeDef",
     "DatasetPropertiesTypeDef",
     "DeleteDocumentClassifierRequestRequestTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEntityRecognizerRequestRequestTypeDef",
     "DeleteFlywheelRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
@@ -116,98 +115,91 @@
     "DescribeEntityRecognizerRequestRequestTypeDef",
     "DescribeEventsDetectionJobRequestRequestTypeDef",
     "DescribeFlywheelIterationRequestRequestTypeDef",
     "DescribeFlywheelRequestRequestTypeDef",
     "DescribeKeyPhrasesDetectionJobRequestRequestTypeDef",
     "DescribePiiEntitiesDetectionJobRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTargetedSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTopicsDetectionJobRequestRequestTypeDef",
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
+    "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
-    "DocumentClassificationJobFilterTypeDef",
     "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
-    "DocumentClassifierFilterTypeDef",
+    "DocumentReaderConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
-    "DominantLanguageDetectionJobFilterTypeDef",
-    "EndpointFilterTypeDef",
-    "EntitiesDetectionJobFilterTypeDef",
     "EntityTypesListItemTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
     "EntityRecognizerDocumentsTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
-    "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
-    "EventsDetectionJobFilterTypeDef",
-    "FlywheelFilterTypeDef",
-    "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
-    "ImportModelResponseTypeDef",
-    "KeyPhrasesDetectionJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    "TopicsDetectionJobFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
-    "RedactionConfigTypeDef",
+    "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "RedactionConfigTypeDef",
+    "StartFlywheelIterationRequestRequestTypeDef",
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
+    "StopEventsDetectionJobRequestRequestTypeDef",
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+    "StopSentimentDetectionJobRequestRequestTypeDef",
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
+    "BatchDetectDominantLanguageItemResultTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateDocumentClassifierResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreateEntityRecognizerResponseTypeDef",
+    "CreateFlywheelResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "DetectDominantLanguageResponseTypeDef",
+    "ImportModelResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
-    "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
     "StartKeyPhrasesDetectionJobResponseTypeDef",
     "StartPiiEntitiesDetectionJobResponseTypeDef",
     "StartSentimentDetectionJobResponseTypeDef",
     "StartTargetedSentimentDetectionJobResponseTypeDef",
     "StartTopicsDetectionJobResponseTypeDef",
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobResponseTypeDef",
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobResponseTypeDef",
-    "StopEventsDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobResponseTypeDef",
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobResponseTypeDef",
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobResponseTypeDef",
-    "StopSentimentDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobResponseTypeDef",
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StopTargetedSentimentDetectionJobResponseTypeDef",
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
-    "BatchDetectDominantLanguageItemResultTypeDef",
-    "DetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesItemResultTypeDef",
     "DetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentItemResultTypeDef",
     "DetectSentimentResponseTypeDef",
     "MentionSentimentTypeDef",
     "BlockReferenceTypeDef",
     "ClassifierMetadataTypeDef",
@@ -217,94 +209,125 @@
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
+    "DataSecurityConfigOutputTypeDef",
+    "VpcConfigUnionTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
-    "ListDatasetsRequestRequestTypeDef",
+    "DatasetFilterTypeDef",
+    "DocumentClassificationJobFilterTypeDef",
+    "DocumentClassifierFilterTypeDef",
+    "DominantLanguageDetectionJobFilterTypeDef",
+    "EndpointFilterTypeDef",
+    "EntitiesDetectionJobFilterTypeDef",
+    "EntityRecognizerFilterTypeDef",
+    "EventsDetectionJobFilterTypeDef",
+    "FlywheelFilterTypeDef",
+    "FlywheelIterationFilterTypeDef",
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    "SentimentDetectionJobFilterTypeDef",
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    "TopicsDetectionJobFilterTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
+    "DocumentClassifierInputDataConfigTypeDef",
+    "DocumentClassifierInputDataConfigOutputTypeDef",
+    "DocumentReaderConfigUnionTypeDef",
+    "InputDataConfigOutputTypeDef",
+    "ListDocumentClassifierSummariesResponseTypeDef",
+    "DocumentMetadataTypeDef",
+    "EntityRecognitionConfigOutputTypeDef",
+    "EntityRecognitionConfigTypeDef",
+    "EntityRecognizerInputDataConfigOutputTypeDef",
+    "EntityRecognizerInputDataConfigTypeDef",
+    "EntityRecognizerMetadataEntityTypesListItemTypeDef",
+    "ListEntityRecognizerSummariesResponseTypeDef",
+    "FlywheelIterationPropertiesTypeDef",
+    "ListFlywheelsResponseTypeDef",
+    "GeometryTypeDef",
+    "SyntaxTokenTypeDef",
+    "RedactionConfigUnionTypeDef",
+    "BatchDetectDominantLanguageResponseTypeDef",
+    "BatchDetectKeyPhrasesResponseTypeDef",
+    "BatchDetectSentimentResponseTypeDef",
+    "TargetedSentimentMentionTypeDef",
+    "EntityTypeDef",
+    "StartDocumentClassificationJobRequestRequestTypeDef",
+    "StartDominantLanguageDetectionJobRequestRequestTypeDef",
+    "StartEntitiesDetectionJobRequestRequestTypeDef",
+    "StartEventsDetectionJobRequestRequestTypeDef",
+    "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
+    "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
+    "StartSentimentDetectionJobRequestRequestTypeDef",
+    "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
+    "StartTopicsDetectionJobRequestRequestTypeDef",
+    "UpdateFlywheelRequestRequestTypeDef",
+    "DataSecurityConfigUnionTypeDef",
+    "DatasetInputDataConfigTypeDef",
+    "ListDatasetsRequestRequestTypeDef",
     "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
-    "DocumentClassifierInputDataConfigTypeDef",
     "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
-    "ListDocumentClassifierSummariesResponseTypeDef",
-    "DocumentMetadataTypeDef",
     "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
-    "EntityRecognitionConfigTypeDef",
-    "EntityRecognizerInputDataConfigTypeDef",
     "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
-    "EntityRecognizerMetadataEntityTypesListItemTypeDef",
-    "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
     "ListFlywheelIterationHistoryRequestRequestTypeDef",
-    "FlywheelIterationPropertiesTypeDef",
-    "ListFlywheelsResponseTypeDef",
-    "GeometryTypeDef",
     "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
-    "SyntaxTokenTypeDef",
-    "BatchDetectDominantLanguageResponseTypeDef",
-    "BatchDetectKeyPhrasesResponseTypeDef",
-    "BatchDetectSentimentResponseTypeDef",
-    "TargetedSentimentMentionTypeDef",
-    "EntityTypeDef",
+    "CreateDocumentClassifierRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigUnionTypeDef",
+    "DocumentClassifierPropertiesTypeDef",
     "DocumentClassificationJobPropertiesTypeDef",
     "DominantLanguageDetectionJobPropertiesTypeDef",
     "EntitiesDetectionJobPropertiesTypeDef",
     "EventsDetectionJobPropertiesTypeDef",
+    "InputDataConfigUnionTypeDef",
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     "PiiEntitiesDetectionJobPropertiesTypeDef",
     "SentimentDetectionJobPropertiesTypeDef",
-    "StartDocumentClassificationJobRequestRequestTypeDef",
-    "StartDominantLanguageDetectionJobRequestRequestTypeDef",
-    "StartEntitiesDetectionJobRequestRequestTypeDef",
-    "StartEventsDetectionJobRequestRequestTypeDef",
-    "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
-    "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
-    "StartSentimentDetectionJobRequestRequestTypeDef",
-    "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
-    "StartTopicsDetectionJobRequestRequestTypeDef",
     "TargetedSentimentDetectionJobPropertiesTypeDef",
     "TopicsDetectionJobPropertiesTypeDef",
-    "UpdateFlywheelRequestRequestTypeDef",
-    "DatasetInputDataConfigTypeDef",
-    "CreateDocumentClassifierRequestRequestTypeDef",
-    "DocumentClassifierPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
+    "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
+    "EntityRecognizerInputDataConfigUnionTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -315,32 +338,56 @@
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
-    "CreateFlywheelRequestRequestTypeDef",
     "FlywheelPropertiesTypeDef",
+    "CreateFlywheelRequestRequestTypeDef",
+    "TaskConfigUnionTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
     "UpdateFlywheelResponseTypeDef",
     "DescribeEntityRecognizerResponseTypeDef",
     "ListEntityRecognizersResponseTypeDef",
     "BatchDetectTargetedSentimentResponseTypeDef",
 )
 
+_RequiredAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_RequiredAugmentedManifestsListItemOutputTypeDef",
+    {
+        "S3Uri": str,
+        "AttributeNames": List[str],
+    },
+)
+_OptionalAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_OptionalAugmentedManifestsListItemOutputTypeDef",
+    {
+        "Split": SplitType,
+        "AnnotationDataS3Uri": str,
+        "SourceDocumentsS3Uri": str,
+        "DocumentType": AugmentedManifestsDocumentTypeFormatType,
+    },
+    total=False,
+)
+
+
+class AugmentedManifestsListItemOutputTypeDef(
+    _RequiredAugmentedManifestsListItemOutputTypeDef,
+    _OptionalAugmentedManifestsListItemOutputTypeDef,
+):
+    pass
+
+
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -384,14 +431,25 @@
         "Index": int,
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
 BatchDetectEntitiesRequestRequestTypeDef = TypedDict(
     "BatchDetectEntitiesRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -446,14 +504,15 @@
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChildBlockTypeDef = TypedDict(
     "ChildBlockTypeDef",
     {
         "ChildBlockId": str,
         "BeginOffset": int,
         "EndOffset": int,
     },
@@ -598,22 +657,14 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -624,45 +675,19 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
-CreateDocumentClassifierResponseTypeDef = TypedDict(
-    "CreateDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityRecognizerResponseTypeDef = TypedDict(
-    "CreateEntityRecognizerResponseTypeDef",
-    {
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlywheelResponseTypeDef = TypedDict(
-    "CreateFlywheelResponseTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
     },
 )
 
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
@@ -741,25 +766,15 @@
 DatasetEntityRecognizerEntityListTypeDef = TypedDict(
     "DatasetEntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
-DatasetFilterTypeDef = TypedDict(
-    "DatasetFilterTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "DatasetType": DatasetTypeType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DatasetPropertiesTypeDef = TypedDict(
     "DatasetPropertiesTypeDef",
     {
         "DatasetArn": str,
         "DatasetName": str,
         "DatasetType": DatasetTypeType,
         "DatasetS3Uri": str,
@@ -930,25 +945,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "ResourcePolicy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1020,14 +1024,36 @@
     "DetectTargetedSentimentRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
 
+_RequiredDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentClassificationConfigOutputTypeDef",
+    {
+        "Mode": DocumentClassifierModeType,
+    },
+)
+_OptionalDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentClassificationConfigOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+    total=False,
+)
+
+
+class DocumentClassificationConfigOutputTypeDef(
+    _RequiredDocumentClassificationConfigOutputTypeDef,
+    _OptionalDocumentClassificationConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
@@ -1041,25 +1067,14 @@
 
 class DocumentClassificationConfigTypeDef(
     _RequiredDocumentClassificationConfigTypeDef, _OptionalDocumentClassificationConfigTypeDef
 ):
     pass
 
 
-DocumentClassificationJobFilterTypeDef = TypedDict(
-    "DocumentClassificationJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
@@ -1092,25 +1107,36 @@
 
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
 
-DocumentClassifierFilterTypeDef = TypedDict(
-    "DocumentClassifierFilterTypeDef",
+_RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentReaderConfigOutputTypeDef",
     {
-        "Status": ModelStatusType,
-        "DocumentClassifierName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
+        "DocumentReadAction": DocumentReadActionType,
+    },
+)
+_OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentReaderConfigOutputTypeDef",
+    {
+        "DocumentReadMode": DocumentReadModeType,
+        "FeatureTypes": List[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
+
+class DocumentReaderConfigOutputTypeDef(
+    _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
+):
+    pass
+
+
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1124,47 +1150,14 @@
     {
         "Page": int,
         "Count": int,
     },
     total=False,
 )
 
-DominantLanguageDetectionJobFilterTypeDef = TypedDict(
-    "DominantLanguageDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EndpointFilterTypeDef = TypedDict(
-    "EndpointFilterTypeDef",
-    {
-        "ModelArn": str,
-        "Status": EndpointStatusType,
-        "CreationTimeBefore": Union[datetime, str],
-        "CreationTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EntitiesDetectionJobFilterTypeDef = TypedDict(
-    "EntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
@@ -1224,25 +1217,14 @@
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
     total=False,
 )
 
-EntityRecognizerFilterTypeDef = TypedDict(
-    "EntityRecognizerFilterTypeDef",
-    {
-        "Status": ModelStatusType,
-        "RecognizerName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesEvaluationMetricsTypeDef = TypedDict(
     "EntityTypesEvaluationMetricsTypeDef",
     {
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
@@ -1265,44 +1247,14 @@
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
         "LatestVersionStatus": ModelStatusType,
     },
     total=False,
 )
 
-EventsDetectionJobFilterTypeDef = TypedDict(
-    "EventsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelFilterTypeDef = TypedDict(
-    "FlywheelFilterTypeDef",
-    {
-        "Status": FlywheelStatusType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelIterationFilterTypeDef = TypedDict(
-    "FlywheelIterationFilterTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 FlywheelModelEvaluationMetricsTypeDef = TypedDict(
     "FlywheelModelEvaluationMetricsTypeDef",
     {
         "AverageF1Score": float,
         "AveragePrecision": float,
         "AverageRecall": float,
         "AverageAccuracy": float,
@@ -1331,29 +1283,20 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
-ImportModelResponseTypeDef = TypedDict(
-    "ImportModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDocumentClassifierSummariesRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     {
@@ -1368,75 +1311,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-SentimentDetectionJobFilterTypeDef = TypedDict(
-    "SentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-TopicsDetectionJobFilterTypeDef = TypedDict(
-    "TopicsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
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
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1459,16 +1348,16 @@
 
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
 
-RedactionConfigTypeDef = TypedDict(
-    "RedactionConfigTypeDef",
+RedactionConfigOutputTypeDef = TypedDict(
+    "RedactionConfigOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
@@ -1491,336 +1380,396 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+RedactionConfigTypeDef = TypedDict(
+    "RedactionConfigTypeDef",
     {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
+        "MaskMode": PiiEntitiesDetectionMaskModeType,
+        "MaskCharacter": str,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FlywheelArn": str,
+    },
+)
+_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
     },
+    total=False,
 )
 
-StartDocumentClassificationJobResponseTypeDef = TypedDict(
-    "StartDocumentClassificationJobResponseTypeDef",
+
+class StartFlywheelIterationRequestRequestTypeDef(
+    _RequiredStartFlywheelIterationRequestRequestTypeDef,
+    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+):
+    pass
+
+
+StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StartDominantLanguageDetectionJobResponseTypeDef",
+StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionJobResponseTypeDef",
+StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEventsDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEventsDetectionJobResponseTypeDef = TypedDict(
-    "StartEventsDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
+StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "FlywheelArn": str,
+        "JobId": str,
     },
 )
-_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+
+StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     {
-        "ClientRequestToken": str,
+        "JobId": str,
+    },
+)
+
+StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    {
+        "JobId": str,
+    },
+)
+
+StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    {
+        "DocumentClassifierArn": str,
+    },
+)
+
+StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    {
+        "EntityRecognizerArn": str,
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
+    {
+        "DesiredModelArn": str,
+        "DesiredInferenceUnits": int,
+        "DesiredDataAccessRoleArn": str,
+        "FlywheelArn": str,
     },
     total=False,
 )
 
 
-class StartFlywheelIterationRequestRequestTypeDef(
-    _RequiredStartFlywheelIterationRequestRequestTypeDef,
-    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
 
-StartFlywheelIterationResponseTypeDef = TypedDict(
-    "StartFlywheelIterationResponseTypeDef",
+BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
+    "BatchDetectDominantLanguageItemResultTypeDef",
     {
-        "FlywheelArn": str,
-        "FlywheelIterationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Index": int,
+        "Languages": List[DominantLanguageTypeDef],
     },
+    total=False,
 )
 
-StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StartKeyPhrasesDetectionJobResponseTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartPiiEntitiesDetectionJobResponseTypeDef",
+CreateDocumentClassifierResponseTypeDef = TypedDict(
+    "CreateDocumentClassifierResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartSentimentDetectionJobResponseTypeDef",
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EndpointArn": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartTargetedSentimentDetectionJobResponseTypeDef",
+CreateEntityRecognizerResponseTypeDef = TypedDict(
+    "CreateEntityRecognizerResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTopicsDetectionJobResponseTypeDef = TypedDict(
-    "StartTopicsDetectionJobResponseTypeDef",
+CreateFlywheelResponseTypeDef = TypedDict(
+    "CreateFlywheelResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobResponseTypeDef",
+DetectDominantLanguageResponseTypeDef = TypedDict(
+    "DetectDominantLanguageResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Languages": List[DominantLanguageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
+ImportModelResponseTypeDef = TypedDict(
+    "ImportModelResponseTypeDef",
     {
-        "JobId": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionJobResponseTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEventsDetectionJobRequestRequestTypeDef",
+StartDocumentClassificationJobResponseTypeDef = TypedDict(
+    "StartDocumentClassificationJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobResponseTypeDef = TypedDict(
-    "StopEventsDetectionJobResponseTypeDef",
+StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StartDominantLanguageDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+StartEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobResponseTypeDef",
+StartEventsDetectionJobResponseTypeDef = TypedDict(
+    "StartEventsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+StartFlywheelIterationResponseTypeDef = TypedDict(
+    "StartFlywheelIterationResponseTypeDef",
     {
-        "JobId": str,
+        "FlywheelArn": str,
+        "FlywheelIterationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobResponseTypeDef",
+StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StartKeyPhrasesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopSentimentDetectionJobRequestRequestTypeDef",
+StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartPiiEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopSentimentDetectionJobResponseTypeDef",
+StartSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartTargetedSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobResponseTypeDef",
+StartTopicsDetectionJobResponseTypeDef = TypedDict(
+    "StartTopicsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobResponseTypeDef",
     {
-        "DocumentClassifierArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+StopEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionJobResponseTypeDef",
     {
-        "EntityRecognizerArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StopEventsDetectionJobResponseTypeDef = TypedDict(
+    "StopEventsDetectionJobResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobResponseTypeDef",
     {
-        "EndpointArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+
+StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "DesiredInferenceUnits": int,
-        "DesiredDataAccessRoleArn": str,
-        "FlywheelArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
-):
-    pass
-
-
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+StopSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopSentimentDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
-    "BatchDetectDominantLanguageItemResultTypeDef",
+StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobResponseTypeDef",
     {
-        "Index": int,
-        "Languages": List[DominantLanguageTypeDef],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-DetectDominantLanguageResponseTypeDef = TypedDict(
-    "DetectDominantLanguageResponseTypeDef",
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
-        "Languages": List[DominantLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DesiredModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesItemResultTypeDef = TypedDict(
     "BatchDetectKeyPhrasesItemResultTypeDef",
     {
         "Index": int,
@@ -1829,15 +1778,15 @@
     total=False,
 )
 
 DetectKeyPhrasesResponseTypeDef = TypedDict(
     "DetectKeyPhrasesResponseTypeDef",
     {
         "KeyPhrases": List[KeyPhraseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentItemResultTypeDef = TypedDict(
     "BatchDetectSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -1848,15 +1797,15 @@
 )
 
 DetectSentimentResponseTypeDef = TypedDict(
     "DetectSentimentResponseTypeDef",
     {
         "Sentiment": SentimentTypeType,
         "SentimentScore": SentimentScoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MentionSentimentTypeDef = TypedDict(
     "MentionSentimentTypeDef",
     {
         "Sentiment": SentimentTypeType,
@@ -1893,15 +1842,15 @@
         "EndpointArn": str,
     },
 )
 _OptionalClassifyDocumentRequestRequestTypeDef = TypedDict(
     "_OptionalClassifyDocumentRequestRequestTypeDef",
     {
         "Text": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
 
 class ClassifyDocumentRequestRequestTypeDef(
@@ -1912,15 +1861,15 @@
 
 DetectEntitiesRequestRequestTypeDef = TypedDict(
     "DetectEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
         "EndpointArn": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
@@ -1942,15 +1891,15 @@
     pass
 
 
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
@@ -2002,15 +1951,15 @@
 
 
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
@@ -2035,14 +1984,26 @@
         "ModelKmsKeyId": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
+DataSecurityConfigOutputTypeDef = TypedDict(
+    "DataSecurityConfigOutputTypeDef",
+    {
+        "ModelKmsKeyId": str,
+        "VolumeKmsKeyId": str,
+        "DataLakeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2058,84 +2019,216 @@
 class DatasetEntityRecognizerInputDataConfigTypeDef(
     _RequiredDatasetEntityRecognizerInputDataConfigTypeDef,
     _OptionalDatasetEntityRecognizerInputDataConfigTypeDef,
 ):
     pass
 
 
-ListDatasetsRequestRequestTypeDef = TypedDict(
-    "ListDatasetsRequestRequestTypeDef",
+DatasetFilterTypeDef = TypedDict(
+    "DatasetFilterTypeDef",
     {
-        "FlywheelArn": str,
-        "Filter": DatasetFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "Status": DatasetStatusType,
+        "DatasetType": DatasetTypeType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassificationJobFilterTypeDef = TypedDict(
+    "DocumentClassificationJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassifierFilterTypeDef = TypedDict(
+    "DocumentClassifierFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "DocumentClassifierName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobFilterTypeDef = TypedDict(
+    "DominantLanguageDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EndpointFilterTypeDef = TypedDict(
+    "EndpointFilterTypeDef",
+    {
+        "ModelArn": str,
+        "Status": EndpointStatusType,
+        "CreationTimeBefore": TimestampTypeDef,
+        "CreationTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobFilterTypeDef = TypedDict(
+    "EntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntityRecognizerFilterTypeDef = TypedDict(
+    "EntityRecognizerFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "RecognizerName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventsDetectionJobFilterTypeDef = TypedDict(
+    "EventsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelFilterTypeDef = TypedDict(
+    "FlywheelFilterTypeDef",
+    {
+        "Status": FlywheelStatusType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelIterationFilterTypeDef = TypedDict(
+    "FlywheelIterationFilterTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+SentimentDetectionJobFilterTypeDef = TypedDict(
+    "SentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobFilterTypeDef = TypedDict(
+    "TopicsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetProperties": DatasetPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "DatasetPropertiesList": List[DatasetPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "EndpointProperties": EndpointPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "EndpointPropertiesList": List[EndpointPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectPiiEntitiesResponseTypeDef = TypedDict(
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
-)
-
-ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestRequestTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
 )
 
 DocumentClassifierInputDataConfigTypeDef = TypedDict(
     "DocumentClassifierInputDataConfigTypeDef",
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
@@ -2145,116 +2238,111 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
+    "DocumentClassifierInputDataConfigOutputTypeDef",
     {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "DataFormat": DocumentClassifierDataFormatType,
+        "S3Uri": str,
+        "TestS3Uri": str,
+        "LabelDelimiter": str,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
+        "DocumentType": DocumentClassifierDocumentTypeFormatType,
+        "Documents": DocumentClassifierDocumentsTypeDef,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestRequestTypeDef",
+DocumentReaderConfigUnionTypeDef = Union[
+    DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
+]
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
     {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "S3Uri": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "InputFormat": InputFormatType,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
+    pass
+
+
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+EntityRecognitionConfigOutputTypeDef = TypedDict(
+    "EntityRecognitionConfigOutputTypeDef",
     {
-        "Filter": DominantLanguageDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
-    total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+EntityRecognitionConfigTypeDef = TypedDict(
+    "EntityRecognitionConfigTypeDef",
     {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
-    total=False,
 )
 
-ListEndpointsRequestRequestTypeDef = TypedDict(
-    "ListEndpointsRequestRequestTypeDef",
+_RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
     {
-        "Filter": EndpointFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
-    total=False,
 )
-
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+_OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
     {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "DataFormat": EntityRecognizerDataFormatType,
+        "Documents": EntityRecognizerDocumentsTypeDef,
+        "Annotations": EntityRecognizerAnnotationsTypeDef,
+        "EntityList": EntityRecognizerEntityListTypeDef,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
     },
     total=False,
 )
 
-ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
 
-EntityRecognitionConfigTypeDef = TypedDict(
-    "EntityRecognitionConfigTypeDef",
-    {
-        "EntityTypes": Sequence[EntityTypesListItemTypeDef],
-    },
-)
+class EntityRecognizerInputDataConfigOutputTypeDef(
+    _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
+    _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
+):
+    pass
+
 
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
@@ -2273,33 +2361,14 @@
 
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
 
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListEntityRecognizersRequestRequestTypeDef = TypedDict(
-    "ListEntityRecognizersRequestRequestTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 EntityRecognizerMetadataEntityTypesListItemTypeDef = TypedDict(
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     {
         "Type": str,
         "EvaluationMetrics": EntityTypesEvaluationMetricsTypeDef,
         "NumberOfTrainMentions": int,
     },
@@ -2307,62 +2376,18 @@
 )
 
 ListEntityRecognizerSummariesResponseTypeDef = TypedDict(
     "ListEntityRecognizerSummariesResponseTypeDef",
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEventsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EventsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListFlywheelsRequestRequestTypeDef = TypedDict(
-    "ListFlywheelsRequestRequestTypeDef",
-    {
-        "Filter": FlywheelFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-    },
-)
-_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "Filter": FlywheelIterationFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListFlywheelIterationHistoryRequestRequestTypeDef(
-    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
-    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 FlywheelIterationPropertiesTypeDef = TypedDict(
     "FlywheelIterationPropertiesTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2378,149 +2403,64 @@
 )
 
 ListFlywheelsResponseTypeDef = TypedDict(
     "ListFlywheelsResponseTypeDef",
     {
         "FlywheelSummaryList": List[FlywheelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 SyntaxTokenTypeDef = TypedDict(
     "SyntaxTokenTypeDef",
     {
         "TokenId": int,
         "Text": str,
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
+RedactionConfigUnionTypeDef = Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef]
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesResponseTypeDef = TypedDict(
     "BatchDetectKeyPhrasesResponseTypeDef",
     {
         "ResultList": List[BatchDetectKeyPhrasesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentResponseTypeDef = TypedDict(
     "BatchDetectSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentMentionTypeDef = TypedDict(
     "TargetedSentimentMentionTypeDef",
     {
         "Score": float,
@@ -2543,155 +2483,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
-DocumentClassificationJobPropertiesTypeDef = TypedDict(
-    "DocumentClassificationJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "DocumentClassifierArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-EntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "EntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "EntityRecognizerArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-EventsDetectionJobPropertiesTypeDef = TypedDict(
-    "EventsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "TargetEventTypes": List[str],
-    },
-    total=False,
-)
-
-KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": PiiOutputDataConfigTypeDef,
-        "RedactionConfig": RedactionConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "Mode": PiiEntitiesDetectionModeType,
-    },
-    total=False,
-)
-
-SentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "SentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartDocumentClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentClassificationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2946,54 +2745,14 @@
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
 
-TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-TopicsDetectionJobPropertiesTypeDef = TypedDict(
-    "TopicsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "NumberOfTopics": int,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -3009,25 +2768,283 @@
 
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
 
+DataSecurityConfigUnionTypeDef = Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef]
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
     },
     total=False,
 )
 
+ListDatasetsRequestRequestTypeDef = TypedDict(
+    "ListDatasetsRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "Filter": DatasetFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": DominantLanguageDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEndpointsRequestRequestTypeDef = TypedDict(
+    "ListEndpointsRequestRequestTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestRequestTypeDef = TypedDict(
+    "ListEntityRecognizersRequestRequestTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEventsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EventsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListFlywheelsRequestRequestTypeDef = TypedDict(
+    "ListFlywheelsRequestRequestTypeDef",
+    {
+        "Filter": FlywheelFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+    },
+)
+_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "Filter": FlywheelIterationFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListFlywheelIterationHistoryRequestRequestTypeDef(
+    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
+    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
     {
         "DocumentClassifierName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -3053,53 +3070,258 @@
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
 
+DocumentClassifierInputDataConfigUnionTypeDef = Union[
+    DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
+]
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
+        "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
         "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+DocumentClassificationJobPropertiesTypeDef = TypedDict(
+    "DocumentClassificationJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "DocumentClassifierArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "EntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "EntityRecognizerArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+EventsDetectionJobPropertiesTypeDef = TypedDict(
+    "EventsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "TargetEventTypes": List[str],
+    },
+    total=False,
+)
+
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
+KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": PiiOutputDataConfigTypeDef,
+        "RedactionConfig": RedactionConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "Mode": PiiEntitiesDetectionModeType,
+    },
+    total=False,
+)
+
+SentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "SentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobPropertiesTypeDef = TypedDict(
+    "TopicsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "NumberOfTopics": int,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTaskConfigOutputTypeDef = TypedDict(
+    "_RequiredTaskConfigOutputTypeDef",
+    {
+        "LanguageCode": LanguageCodeType,
+    },
+)
+_OptionalTaskConfigOutputTypeDef = TypedDict(
+    "_OptionalTaskConfigOutputTypeDef",
+    {
+        "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
+        "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
     },
+    total=False,
 )
 
+
+class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
+    pass
+
+
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3143,14 +3365,17 @@
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
 
+EntityRecognizerInputDataConfigUnionTypeDef = Union[
+    EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
+]
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3158,24 +3383,24 @@
     total=False,
 )
 
 DescribeFlywheelIterationResponseTypeDef = TypedDict(
     "DescribeFlywheelIterationResponseTypeDef",
     {
         "FlywheelIterationProperties": FlywheelIterationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFlywheelIterationHistoryResponseTypeDef = TypedDict(
     "ListFlywheelIterationHistoryResponseTypeDef",
     {
         "FlywheelIterationPropertiesList": List[FlywheelIterationPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "Id": str,
@@ -3197,15 +3422,15 @@
     total=False,
 )
 
 DetectSyntaxResponseTypeDef = TypedDict(
     "DetectSyntaxResponseTypeDef",
     {
         "SyntaxTokens": List[SyntaxTokenTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentEntityTypeDef = TypedDict(
     "TargetedSentimentEntityTypeDef",
     {
         "DescriptiveMentionIndex": List[int],
@@ -3219,214 +3444,233 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "DatasetName": str,
+        "InputDataConfig": DatasetInputDataConfigTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentClassificationJobsResponseTypeDef = TypedDict(
     "ListDocumentClassificationJobsResponseTypeDef",
     {
         "DocumentClassificationJobPropertiesList": List[DocumentClassificationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDominantLanguageDetectionJobResponseTypeDef = TypedDict(
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     {
         "DominantLanguageDetectionJobProperties": DominantLanguageDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDominantLanguageDetectionJobsResponseTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     {
         "DominantLanguageDetectionJobPropertiesList": List[
             DominantLanguageDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionJobResponseTypeDef",
     {
         "EntitiesDetectionJobProperties": EntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionJobsResponseTypeDef",
     {
         "EntitiesDetectionJobPropertiesList": List[EntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsDetectionJobResponseTypeDef = TypedDict(
     "DescribeEventsDetectionJobResponseTypeDef",
     {
         "EventsDetectionJobProperties": EventsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventsDetectionJobsResponseTypeDef = TypedDict(
     "ListEventsDetectionJobsResponseTypeDef",
     {
         "EventsDetectionJobPropertiesList": List[EventsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
     "DescribeKeyPhrasesDetectionJobResponseTypeDef",
     {
         "KeyPhrasesDetectionJobProperties": KeyPhrasesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeyPhrasesDetectionJobsResponseTypeDef = TypedDict(
     "ListKeyPhrasesDetectionJobsResponseTypeDef",
     {
         "KeyPhrasesDetectionJobPropertiesList": List[KeyPhrasesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePiiEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribePiiEntitiesDetectionJobResponseTypeDef",
     {
         "PiiEntitiesDetectionJobProperties": PiiEntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPiiEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     {
         "PiiEntitiesDetectionJobPropertiesList": List[PiiEntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeSentimentDetectionJobResponseTypeDef",
     {
         "SentimentDetectionJobProperties": SentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListSentimentDetectionJobsResponseTypeDef",
     {
         "SentimentDetectionJobPropertiesList": List[SentimentDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     {
         "TargetedSentimentDetectionJobProperties": TargetedSentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetedSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     {
         "TargetedSentimentDetectionJobPropertiesList": List[
             TargetedSentimentDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTopicsDetectionJobResponseTypeDef = TypedDict(
     "DescribeTopicsDetectionJobResponseTypeDef",
     {
         "TopicsDetectionJobProperties": TopicsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicsDetectionJobsResponseTypeDef = TypedDict(
     "ListTopicsDetectionJobsResponseTypeDef",
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
+FlywheelPropertiesTypeDef = TypedDict(
+    "FlywheelPropertiesTypeDef",
     {
         "FlywheelArn": str,
-        "DatasetName": str,
-        "InputDataConfig": DatasetInputDataConfigTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "Description": str,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "ActiveModelArn": str,
+        "DataAccessRoleArn": str,
+        "TaskConfig": TaskConfigOutputTypeDef,
+        "DataLakeS3Uri": str,
+        "DataSecurityConfig": DataSecurityConfigOutputTypeDef,
+        "Status": FlywheelStatusType,
+        "ModelType": ModelTypeType,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LatestFlywheelIteration": str,
     },
     total=False,
 )
 
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3447,49 +3691,31 @@
 
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
 
-FlywheelPropertiesTypeDef = TypedDict(
-    "FlywheelPropertiesTypeDef",
-    {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "DataAccessRoleArn": str,
-        "TaskConfig": TaskConfigTypeDef,
-        "DataLakeS3Uri": str,
-        "DataSecurityConfig": DataSecurityConfigTypeDef,
-        "Status": FlywheelStatusType,
-        "ModelType": ModelTypeType,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LatestFlywheelIteration": str,
-    },
-    total=False,
-)
-
+TaskConfigUnionTypeDef = Union[TaskConfigTypeDef, TaskConfigOutputTypeDef]
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
+        "InputDataConfig": EntityRecognizerInputDataConfigOutputTypeDef,
         "RecognizerMetadata": EntityRecognizerMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
         "OutputDataConfig": EntityRecognizerOutputDataConfigTypeDef,
     },
     total=False,
@@ -3499,24 +3725,24 @@
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Blocks": List[BlockTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSyntaxResponseTypeDef = TypedDict(
     "BatchDetectSyntaxResponseTypeDef",
     {
         "ResultList": List[BatchDetectSyntaxItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentItemResultTypeDef = TypedDict(
     "BatchDetectTargetedSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -3525,61 +3751,61 @@
     total=False,
 )
 
 DetectTargetedSentimentResponseTypeDef = TypedDict(
     "DetectTargetedSentimentResponseTypeDef",
     {
         "Entities": List[TargetedSentimentEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectEntitiesResponseTypeDef = TypedDict(
     "BatchDetectEntitiesResponseTypeDef",
     {
         "ResultList": List[BatchDetectEntitiesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFlywheelResponseTypeDef = TypedDict(
     "DescribeFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlywheelResponseTypeDef = TypedDict(
     "UpdateFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityRecognizerResponseTypeDef = TypedDict(
     "DescribeEntityRecognizerResponseTypeDef",
     {
         "EntityRecognizerProperties": EntityRecognizerPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntityRecognizersResponseTypeDef = TypedDict(
     "ListEntityRecognizersResponseTypeDef",
     {
         "EntityRecognizerPropertiesList": List[EntityRecognizerPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentResponseTypeDef = TypedDict(
     "BatchDetectTargetedSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectTargetedSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend/type_defs.pyi` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for comprehend service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemTypeDef
+    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
 
-    data: AugmentedManifestsListItemTypeDef = {...}
+    data: AugmentedManifestsListItemOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -58,51 +58,50 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
+    "BlobTypeDef",
     "ChildBlockTypeDef",
     "RelationshipsListItemTypeDef",
     "BoundingBoxTypeDef",
     "ClassifierEvaluationMetricsTypeDef",
     "DocumentReaderConfigTypeDef",
     "DocumentClassTypeDef",
     "DocumentLabelTypeDef",
     "DocumentTypeListItemTypeDef",
     "ErrorsListItemTypeDef",
     "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
-    "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
-    "CreateDocumentClassifierResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreateEntityRecognizerResponseTypeDef",
-    "CreateFlywheelResponseTypeDef",
+    "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
-    "DatasetFilterTypeDef",
+    "TimestampTypeDef",
     "DatasetPropertiesTypeDef",
     "DeleteDocumentClassifierRequestRequestTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEntityRecognizerRequestRequestTypeDef",
     "DeleteFlywheelRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
@@ -115,98 +114,91 @@
     "DescribeEntityRecognizerRequestRequestTypeDef",
     "DescribeEventsDetectionJobRequestRequestTypeDef",
     "DescribeFlywheelIterationRequestRequestTypeDef",
     "DescribeFlywheelRequestRequestTypeDef",
     "DescribeKeyPhrasesDetectionJobRequestRequestTypeDef",
     "DescribePiiEntitiesDetectionJobRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTargetedSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTopicsDetectionJobRequestRequestTypeDef",
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
+    "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
-    "DocumentClassificationJobFilterTypeDef",
     "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
-    "DocumentClassifierFilterTypeDef",
+    "DocumentReaderConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
-    "DominantLanguageDetectionJobFilterTypeDef",
-    "EndpointFilterTypeDef",
-    "EntitiesDetectionJobFilterTypeDef",
     "EntityTypesListItemTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
     "EntityRecognizerDocumentsTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
-    "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
-    "EventsDetectionJobFilterTypeDef",
-    "FlywheelFilterTypeDef",
-    "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
-    "ImportModelResponseTypeDef",
-    "KeyPhrasesDetectionJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    "TopicsDetectionJobFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
-    "RedactionConfigTypeDef",
+    "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "RedactionConfigTypeDef",
+    "StartFlywheelIterationRequestRequestTypeDef",
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
+    "StopEventsDetectionJobRequestRequestTypeDef",
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+    "StopSentimentDetectionJobRequestRequestTypeDef",
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
+    "BatchDetectDominantLanguageItemResultTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateDocumentClassifierResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreateEntityRecognizerResponseTypeDef",
+    "CreateFlywheelResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "DetectDominantLanguageResponseTypeDef",
+    "ImportModelResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
-    "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
     "StartKeyPhrasesDetectionJobResponseTypeDef",
     "StartPiiEntitiesDetectionJobResponseTypeDef",
     "StartSentimentDetectionJobResponseTypeDef",
     "StartTargetedSentimentDetectionJobResponseTypeDef",
     "StartTopicsDetectionJobResponseTypeDef",
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobResponseTypeDef",
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobResponseTypeDef",
-    "StopEventsDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobResponseTypeDef",
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobResponseTypeDef",
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobResponseTypeDef",
-    "StopSentimentDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobResponseTypeDef",
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StopTargetedSentimentDetectionJobResponseTypeDef",
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
-    "BatchDetectDominantLanguageItemResultTypeDef",
-    "DetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesItemResultTypeDef",
     "DetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentItemResultTypeDef",
     "DetectSentimentResponseTypeDef",
     "MentionSentimentTypeDef",
     "BlockReferenceTypeDef",
     "ClassifierMetadataTypeDef",
@@ -216,94 +208,125 @@
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
+    "DataSecurityConfigOutputTypeDef",
+    "VpcConfigUnionTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
-    "ListDatasetsRequestRequestTypeDef",
+    "DatasetFilterTypeDef",
+    "DocumentClassificationJobFilterTypeDef",
+    "DocumentClassifierFilterTypeDef",
+    "DominantLanguageDetectionJobFilterTypeDef",
+    "EndpointFilterTypeDef",
+    "EntitiesDetectionJobFilterTypeDef",
+    "EntityRecognizerFilterTypeDef",
+    "EventsDetectionJobFilterTypeDef",
+    "FlywheelFilterTypeDef",
+    "FlywheelIterationFilterTypeDef",
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    "SentimentDetectionJobFilterTypeDef",
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    "TopicsDetectionJobFilterTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
+    "DocumentClassifierInputDataConfigTypeDef",
+    "DocumentClassifierInputDataConfigOutputTypeDef",
+    "DocumentReaderConfigUnionTypeDef",
+    "InputDataConfigOutputTypeDef",
+    "ListDocumentClassifierSummariesResponseTypeDef",
+    "DocumentMetadataTypeDef",
+    "EntityRecognitionConfigOutputTypeDef",
+    "EntityRecognitionConfigTypeDef",
+    "EntityRecognizerInputDataConfigOutputTypeDef",
+    "EntityRecognizerInputDataConfigTypeDef",
+    "EntityRecognizerMetadataEntityTypesListItemTypeDef",
+    "ListEntityRecognizerSummariesResponseTypeDef",
+    "FlywheelIterationPropertiesTypeDef",
+    "ListFlywheelsResponseTypeDef",
+    "GeometryTypeDef",
+    "SyntaxTokenTypeDef",
+    "RedactionConfigUnionTypeDef",
+    "BatchDetectDominantLanguageResponseTypeDef",
+    "BatchDetectKeyPhrasesResponseTypeDef",
+    "BatchDetectSentimentResponseTypeDef",
+    "TargetedSentimentMentionTypeDef",
+    "EntityTypeDef",
+    "StartDocumentClassificationJobRequestRequestTypeDef",
+    "StartDominantLanguageDetectionJobRequestRequestTypeDef",
+    "StartEntitiesDetectionJobRequestRequestTypeDef",
+    "StartEventsDetectionJobRequestRequestTypeDef",
+    "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
+    "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
+    "StartSentimentDetectionJobRequestRequestTypeDef",
+    "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
+    "StartTopicsDetectionJobRequestRequestTypeDef",
+    "UpdateFlywheelRequestRequestTypeDef",
+    "DataSecurityConfigUnionTypeDef",
+    "DatasetInputDataConfigTypeDef",
+    "ListDatasetsRequestRequestTypeDef",
     "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
-    "DocumentClassifierInputDataConfigTypeDef",
     "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
-    "ListDocumentClassifierSummariesResponseTypeDef",
-    "DocumentMetadataTypeDef",
     "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
-    "EntityRecognitionConfigTypeDef",
-    "EntityRecognizerInputDataConfigTypeDef",
     "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
-    "EntityRecognizerMetadataEntityTypesListItemTypeDef",
-    "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
     "ListFlywheelIterationHistoryRequestRequestTypeDef",
-    "FlywheelIterationPropertiesTypeDef",
-    "ListFlywheelsResponseTypeDef",
-    "GeometryTypeDef",
     "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
-    "SyntaxTokenTypeDef",
-    "BatchDetectDominantLanguageResponseTypeDef",
-    "BatchDetectKeyPhrasesResponseTypeDef",
-    "BatchDetectSentimentResponseTypeDef",
-    "TargetedSentimentMentionTypeDef",
-    "EntityTypeDef",
+    "CreateDocumentClassifierRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigUnionTypeDef",
+    "DocumentClassifierPropertiesTypeDef",
     "DocumentClassificationJobPropertiesTypeDef",
     "DominantLanguageDetectionJobPropertiesTypeDef",
     "EntitiesDetectionJobPropertiesTypeDef",
     "EventsDetectionJobPropertiesTypeDef",
+    "InputDataConfigUnionTypeDef",
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     "PiiEntitiesDetectionJobPropertiesTypeDef",
     "SentimentDetectionJobPropertiesTypeDef",
-    "StartDocumentClassificationJobRequestRequestTypeDef",
-    "StartDominantLanguageDetectionJobRequestRequestTypeDef",
-    "StartEntitiesDetectionJobRequestRequestTypeDef",
-    "StartEventsDetectionJobRequestRequestTypeDef",
-    "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
-    "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
-    "StartSentimentDetectionJobRequestRequestTypeDef",
-    "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
-    "StartTopicsDetectionJobRequestRequestTypeDef",
     "TargetedSentimentDetectionJobPropertiesTypeDef",
     "TopicsDetectionJobPropertiesTypeDef",
-    "UpdateFlywheelRequestRequestTypeDef",
-    "DatasetInputDataConfigTypeDef",
-    "CreateDocumentClassifierRequestRequestTypeDef",
-    "DocumentClassifierPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
+    "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
+    "EntityRecognizerInputDataConfigUnionTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -314,32 +337,54 @@
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
-    "CreateFlywheelRequestRequestTypeDef",
     "FlywheelPropertiesTypeDef",
+    "CreateFlywheelRequestRequestTypeDef",
+    "TaskConfigUnionTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
     "UpdateFlywheelResponseTypeDef",
     "DescribeEntityRecognizerResponseTypeDef",
     "ListEntityRecognizersResponseTypeDef",
     "BatchDetectTargetedSentimentResponseTypeDef",
 )
 
+_RequiredAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_RequiredAugmentedManifestsListItemOutputTypeDef",
+    {
+        "S3Uri": str,
+        "AttributeNames": List[str],
+    },
+)
+_OptionalAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_OptionalAugmentedManifestsListItemOutputTypeDef",
+    {
+        "Split": SplitType,
+        "AnnotationDataS3Uri": str,
+        "SourceDocumentsS3Uri": str,
+        "DocumentType": AugmentedManifestsDocumentTypeFormatType,
+    },
+    total=False,
+)
+
+class AugmentedManifestsListItemOutputTypeDef(
+    _RequiredAugmentedManifestsListItemOutputTypeDef,
+    _OptionalAugmentedManifestsListItemOutputTypeDef,
+):
+    pass
+
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -381,14 +426,25 @@
         "Index": int,
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
 BatchDetectEntitiesRequestRequestTypeDef = TypedDict(
     "BatchDetectEntitiesRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -443,14 +499,15 @@
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChildBlockTypeDef = TypedDict(
     "ChildBlockTypeDef",
     {
         "ChildBlockId": str,
         "BeginOffset": int,
         "EndOffset": int,
     },
@@ -591,22 +648,14 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -617,45 +666,19 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
-CreateDocumentClassifierResponseTypeDef = TypedDict(
-    "CreateDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityRecognizerResponseTypeDef = TypedDict(
-    "CreateEntityRecognizerResponseTypeDef",
-    {
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlywheelResponseTypeDef = TypedDict(
-    "CreateFlywheelResponseTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
     },
 )
 
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
@@ -728,25 +751,15 @@
 DatasetEntityRecognizerEntityListTypeDef = TypedDict(
     "DatasetEntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
-DatasetFilterTypeDef = TypedDict(
-    "DatasetFilterTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "DatasetType": DatasetTypeType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DatasetPropertiesTypeDef = TypedDict(
     "DatasetPropertiesTypeDef",
     {
         "DatasetArn": str,
         "DatasetName": str,
         "DatasetType": DatasetTypeType,
         "DatasetS3Uri": str,
@@ -915,25 +928,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "ResourcePolicy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1005,14 +1007,34 @@
     "DetectTargetedSentimentRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
 
+_RequiredDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentClassificationConfigOutputTypeDef",
+    {
+        "Mode": DocumentClassifierModeType,
+    },
+)
+_OptionalDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentClassificationConfigOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+    total=False,
+)
+
+class DocumentClassificationConfigOutputTypeDef(
+    _RequiredDocumentClassificationConfigOutputTypeDef,
+    _OptionalDocumentClassificationConfigOutputTypeDef,
+):
+    pass
+
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
@@ -1024,25 +1046,14 @@
 )
 
 class DocumentClassificationConfigTypeDef(
     _RequiredDocumentClassificationConfigTypeDef, _OptionalDocumentClassificationConfigTypeDef
 ):
     pass
 
-DocumentClassificationJobFilterTypeDef = TypedDict(
-    "DocumentClassificationJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
@@ -1071,25 +1082,34 @@
 )
 
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
-DocumentClassifierFilterTypeDef = TypedDict(
-    "DocumentClassifierFilterTypeDef",
+_RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentReaderConfigOutputTypeDef",
     {
-        "Status": ModelStatusType,
-        "DocumentClassifierName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
+        "DocumentReadAction": DocumentReadActionType,
+    },
+)
+_OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentReaderConfigOutputTypeDef",
+    {
+        "DocumentReadMode": DocumentReadModeType,
+        "FeatureTypes": List[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
+class DocumentReaderConfigOutputTypeDef(
+    _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
+):
+    pass
+
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1103,47 +1123,14 @@
     {
         "Page": int,
         "Count": int,
     },
     total=False,
 )
 
-DominantLanguageDetectionJobFilterTypeDef = TypedDict(
-    "DominantLanguageDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EndpointFilterTypeDef = TypedDict(
-    "EndpointFilterTypeDef",
-    {
-        "ModelArn": str,
-        "Status": EndpointStatusType,
-        "CreationTimeBefore": Union[datetime, str],
-        "CreationTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EntitiesDetectionJobFilterTypeDef = TypedDict(
-    "EntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
@@ -1199,25 +1186,14 @@
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
     total=False,
 )
 
-EntityRecognizerFilterTypeDef = TypedDict(
-    "EntityRecognizerFilterTypeDef",
-    {
-        "Status": ModelStatusType,
-        "RecognizerName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesEvaluationMetricsTypeDef = TypedDict(
     "EntityTypesEvaluationMetricsTypeDef",
     {
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
@@ -1240,44 +1216,14 @@
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
         "LatestVersionStatus": ModelStatusType,
     },
     total=False,
 )
 
-EventsDetectionJobFilterTypeDef = TypedDict(
-    "EventsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelFilterTypeDef = TypedDict(
-    "FlywheelFilterTypeDef",
-    {
-        "Status": FlywheelStatusType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelIterationFilterTypeDef = TypedDict(
-    "FlywheelIterationFilterTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 FlywheelModelEvaluationMetricsTypeDef = TypedDict(
     "FlywheelModelEvaluationMetricsTypeDef",
     {
         "AverageF1Score": float,
         "AveragePrecision": float,
         "AverageRecall": float,
         "AverageAccuracy": float,
@@ -1306,29 +1252,20 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
-ImportModelResponseTypeDef = TypedDict(
-    "ImportModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDocumentClassifierSummariesRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     {
@@ -1343,75 +1280,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-SentimentDetectionJobFilterTypeDef = TypedDict(
-    "SentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-TopicsDetectionJobFilterTypeDef = TypedDict(
-    "TopicsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
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
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1432,16 +1315,16 @@
 )
 
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
-RedactionConfigTypeDef = TypedDict(
-    "RedactionConfigTypeDef",
+RedactionConfigOutputTypeDef = TypedDict(
+    "RedactionConfigOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
@@ -1462,332 +1345,392 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+RedactionConfigTypeDef = TypedDict(
+    "RedactionConfigTypeDef",
     {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
+        "MaskMode": PiiEntitiesDetectionMaskModeType,
+        "MaskCharacter": str,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FlywheelArn": str,
     },
 )
+_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
 
-StartDocumentClassificationJobResponseTypeDef = TypedDict(
-    "StartDocumentClassificationJobResponseTypeDef",
+class StartFlywheelIterationRequestRequestTypeDef(
+    _RequiredStartFlywheelIterationRequestRequestTypeDef,
+    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+):
+    pass
+
+StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StartDominantLanguageDetectionJobResponseTypeDef",
+StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionJobResponseTypeDef",
+StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEventsDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEventsDetectionJobResponseTypeDef = TypedDict(
-    "StartEventsDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
+StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "FlywheelArn": str,
+        "JobId": str,
     },
 )
-_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+
+StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     {
-        "ClientRequestToken": str,
+        "JobId": str,
+    },
+)
+
+StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    {
+        "JobId": str,
+    },
+)
+
+StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    {
+        "DocumentClassifierArn": str,
+    },
+)
+
+StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    {
+        "EntityRecognizerArn": str,
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
+    {
+        "DesiredModelArn": str,
+        "DesiredInferenceUnits": int,
+        "DesiredDataAccessRoleArn": str,
+        "FlywheelArn": str,
     },
     total=False,
 )
 
-class StartFlywheelIterationRequestRequestTypeDef(
-    _RequiredStartFlywheelIterationRequestRequestTypeDef,
-    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
-StartFlywheelIterationResponseTypeDef = TypedDict(
-    "StartFlywheelIterationResponseTypeDef",
+BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
+    "BatchDetectDominantLanguageItemResultTypeDef",
     {
-        "FlywheelArn": str,
-        "FlywheelIterationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Index": int,
+        "Languages": List[DominantLanguageTypeDef],
     },
+    total=False,
 )
 
-StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StartKeyPhrasesDetectionJobResponseTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartPiiEntitiesDetectionJobResponseTypeDef",
+CreateDocumentClassifierResponseTypeDef = TypedDict(
+    "CreateDocumentClassifierResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartSentimentDetectionJobResponseTypeDef",
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EndpointArn": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartTargetedSentimentDetectionJobResponseTypeDef",
+CreateEntityRecognizerResponseTypeDef = TypedDict(
+    "CreateEntityRecognizerResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTopicsDetectionJobResponseTypeDef = TypedDict(
-    "StartTopicsDetectionJobResponseTypeDef",
+CreateFlywheelResponseTypeDef = TypedDict(
+    "CreateFlywheelResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobResponseTypeDef",
+DetectDominantLanguageResponseTypeDef = TypedDict(
+    "DetectDominantLanguageResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Languages": List[DominantLanguageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
+ImportModelResponseTypeDef = TypedDict(
+    "ImportModelResponseTypeDef",
     {
-        "JobId": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionJobResponseTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEventsDetectionJobRequestRequestTypeDef",
+StartDocumentClassificationJobResponseTypeDef = TypedDict(
+    "StartDocumentClassificationJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobResponseTypeDef = TypedDict(
-    "StopEventsDetectionJobResponseTypeDef",
+StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StartDominantLanguageDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+StartEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobResponseTypeDef",
+StartEventsDetectionJobResponseTypeDef = TypedDict(
+    "StartEventsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+StartFlywheelIterationResponseTypeDef = TypedDict(
+    "StartFlywheelIterationResponseTypeDef",
     {
-        "JobId": str,
+        "FlywheelArn": str,
+        "FlywheelIterationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobResponseTypeDef",
+StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StartKeyPhrasesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopSentimentDetectionJobRequestRequestTypeDef",
+StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartPiiEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopSentimentDetectionJobResponseTypeDef",
+StartSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartTargetedSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobResponseTypeDef",
+StartTopicsDetectionJobResponseTypeDef = TypedDict(
+    "StartTopicsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobResponseTypeDef",
     {
-        "DocumentClassifierArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+StopEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionJobResponseTypeDef",
     {
-        "EntityRecognizerArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StopEventsDetectionJobResponseTypeDef = TypedDict(
+    "StopEventsDetectionJobResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobResponseTypeDef",
     {
-        "EndpointArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+
+StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "DesiredInferenceUnits": int,
-        "DesiredDataAccessRoleArn": str,
-        "FlywheelArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
-):
-    pass
-
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+StopSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopSentimentDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
-    "BatchDetectDominantLanguageItemResultTypeDef",
+StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobResponseTypeDef",
     {
-        "Index": int,
-        "Languages": List[DominantLanguageTypeDef],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-DetectDominantLanguageResponseTypeDef = TypedDict(
-    "DetectDominantLanguageResponseTypeDef",
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
-        "Languages": List[DominantLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DesiredModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesItemResultTypeDef = TypedDict(
     "BatchDetectKeyPhrasesItemResultTypeDef",
     {
         "Index": int,
@@ -1796,15 +1739,15 @@
     total=False,
 )
 
 DetectKeyPhrasesResponseTypeDef = TypedDict(
     "DetectKeyPhrasesResponseTypeDef",
     {
         "KeyPhrases": List[KeyPhraseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentItemResultTypeDef = TypedDict(
     "BatchDetectSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -1815,15 +1758,15 @@
 )
 
 DetectSentimentResponseTypeDef = TypedDict(
     "DetectSentimentResponseTypeDef",
     {
         "Sentiment": SentimentTypeType,
         "SentimentScore": SentimentScoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MentionSentimentTypeDef = TypedDict(
     "MentionSentimentTypeDef",
     {
         "Sentiment": SentimentTypeType,
@@ -1860,15 +1803,15 @@
         "EndpointArn": str,
     },
 )
 _OptionalClassifyDocumentRequestRequestTypeDef = TypedDict(
     "_OptionalClassifyDocumentRequestRequestTypeDef",
     {
         "Text": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
 class ClassifyDocumentRequestRequestTypeDef(
     _RequiredClassifyDocumentRequestRequestTypeDef, _OptionalClassifyDocumentRequestRequestTypeDef
@@ -1877,15 +1820,15 @@
 
 DetectEntitiesRequestRequestTypeDef = TypedDict(
     "DetectEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
         "EndpointArn": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
@@ -1905,15 +1848,15 @@
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
@@ -1961,15 +1904,15 @@
     pass
 
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
@@ -1994,14 +1937,26 @@
         "ModelKmsKeyId": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
+DataSecurityConfigOutputTypeDef = TypedDict(
+    "DataSecurityConfigOutputTypeDef",
+    {
+        "ModelKmsKeyId": str,
+        "VolumeKmsKeyId": str,
+        "DataLakeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2015,84 +1970,216 @@
 
 class DatasetEntityRecognizerInputDataConfigTypeDef(
     _RequiredDatasetEntityRecognizerInputDataConfigTypeDef,
     _OptionalDatasetEntityRecognizerInputDataConfigTypeDef,
 ):
     pass
 
-ListDatasetsRequestRequestTypeDef = TypedDict(
-    "ListDatasetsRequestRequestTypeDef",
+DatasetFilterTypeDef = TypedDict(
+    "DatasetFilterTypeDef",
     {
-        "FlywheelArn": str,
-        "Filter": DatasetFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "Status": DatasetStatusType,
+        "DatasetType": DatasetTypeType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassificationJobFilterTypeDef = TypedDict(
+    "DocumentClassificationJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassifierFilterTypeDef = TypedDict(
+    "DocumentClassifierFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "DocumentClassifierName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobFilterTypeDef = TypedDict(
+    "DominantLanguageDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EndpointFilterTypeDef = TypedDict(
+    "EndpointFilterTypeDef",
+    {
+        "ModelArn": str,
+        "Status": EndpointStatusType,
+        "CreationTimeBefore": TimestampTypeDef,
+        "CreationTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobFilterTypeDef = TypedDict(
+    "EntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntityRecognizerFilterTypeDef = TypedDict(
+    "EntityRecognizerFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "RecognizerName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventsDetectionJobFilterTypeDef = TypedDict(
+    "EventsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelFilterTypeDef = TypedDict(
+    "FlywheelFilterTypeDef",
+    {
+        "Status": FlywheelStatusType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelIterationFilterTypeDef = TypedDict(
+    "FlywheelIterationFilterTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+SentimentDetectionJobFilterTypeDef = TypedDict(
+    "SentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobFilterTypeDef = TypedDict(
+    "TopicsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetProperties": DatasetPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "DatasetPropertiesList": List[DatasetPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "EndpointProperties": EndpointPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "EndpointPropertiesList": List[EndpointPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectPiiEntitiesResponseTypeDef = TypedDict(
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestRequestTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DocumentClassifierInputDataConfigTypeDef = TypedDict(
     "DocumentClassifierInputDataConfigTypeDef",
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
@@ -2102,116 +2189,107 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
+    "DocumentClassifierInputDataConfigOutputTypeDef",
     {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "DataFormat": DocumentClassifierDataFormatType,
+        "S3Uri": str,
+        "TestS3Uri": str,
+        "LabelDelimiter": str,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
+        "DocumentType": DocumentClassifierDocumentTypeFormatType,
+        "Documents": DocumentClassifierDocumentsTypeDef,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestRequestTypeDef",
+DocumentReaderConfigUnionTypeDef = Union[
+    DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
+]
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
     {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "S3Uri": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "InputFormat": InputFormatType,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
+    pass
+
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": DominantLanguageDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+EntityRecognitionConfigOutputTypeDef = TypedDict(
+    "EntityRecognitionConfigOutputTypeDef",
     {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
-    total=False,
 )
 
-ListEndpointsRequestRequestTypeDef = TypedDict(
-    "ListEndpointsRequestRequestTypeDef",
+EntityRecognitionConfigTypeDef = TypedDict(
+    "EntityRecognitionConfigTypeDef",
     {
-        "Filter": EndpointFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
-    total=False,
 )
 
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+_RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
     {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
-    total=False,
 )
-
-ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+_OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
     {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "DataFormat": EntityRecognizerDataFormatType,
+        "Documents": EntityRecognizerDocumentsTypeDef,
+        "Annotations": EntityRecognizerAnnotationsTypeDef,
+        "EntityList": EntityRecognizerEntityListTypeDef,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
     },
     total=False,
 )
 
-EntityRecognitionConfigTypeDef = TypedDict(
-    "EntityRecognitionConfigTypeDef",
-    {
-        "EntityTypes": Sequence[EntityTypesListItemTypeDef],
-    },
-)
+class EntityRecognizerInputDataConfigOutputTypeDef(
+    _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
+    _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
+):
+    pass
 
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
@@ -2228,33 +2306,14 @@
 )
 
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListEntityRecognizersRequestRequestTypeDef = TypedDict(
-    "ListEntityRecognizersRequestRequestTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 EntityRecognizerMetadataEntityTypesListItemTypeDef = TypedDict(
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     {
         "Type": str,
         "EvaluationMetrics": EntityTypesEvaluationMetricsTypeDef,
         "NumberOfTrainMentions": int,
     },
@@ -2262,60 +2321,18 @@
 )
 
 ListEntityRecognizerSummariesResponseTypeDef = TypedDict(
     "ListEntityRecognizerSummariesResponseTypeDef",
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEventsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EventsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListFlywheelsRequestRequestTypeDef = TypedDict(
-    "ListFlywheelsRequestRequestTypeDef",
-    {
-        "Filter": FlywheelFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-    },
-)
-_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "Filter": FlywheelIterationFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListFlywheelIterationHistoryRequestRequestTypeDef(
-    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
-    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
-):
-    pass
-
 FlywheelIterationPropertiesTypeDef = TypedDict(
     "FlywheelIterationPropertiesTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2331,149 +2348,64 @@
 )
 
 ListFlywheelsResponseTypeDef = TypedDict(
     "ListFlywheelsResponseTypeDef",
     {
         "FlywheelSummaryList": List[FlywheelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 SyntaxTokenTypeDef = TypedDict(
     "SyntaxTokenTypeDef",
     {
         "TokenId": int,
         "Text": str,
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
+RedactionConfigUnionTypeDef = Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef]
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesResponseTypeDef = TypedDict(
     "BatchDetectKeyPhrasesResponseTypeDef",
     {
         "ResultList": List[BatchDetectKeyPhrasesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentResponseTypeDef = TypedDict(
     "BatchDetectSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentMentionTypeDef = TypedDict(
     "TargetedSentimentMentionTypeDef",
     {
         "Score": float,
@@ -2496,155 +2428,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
-DocumentClassificationJobPropertiesTypeDef = TypedDict(
-    "DocumentClassificationJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "DocumentClassifierArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-EntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "EntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "EntityRecognizerArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-EventsDetectionJobPropertiesTypeDef = TypedDict(
-    "EventsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "TargetEventTypes": List[str],
-    },
-    total=False,
-)
-
-KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": PiiOutputDataConfigTypeDef,
-        "RedactionConfig": RedactionConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "Mode": PiiEntitiesDetectionModeType,
-    },
-    total=False,
-)
-
-SentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "SentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartDocumentClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentClassificationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2881,54 +2672,14 @@
 
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-TopicsDetectionJobPropertiesTypeDef = TypedDict(
-    "TopicsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "NumberOfTopics": int,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -2942,25 +2693,281 @@
 )
 
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
+DataSecurityConfigUnionTypeDef = Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef]
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
     },
     total=False,
 )
 
+ListDatasetsRequestRequestTypeDef = TypedDict(
+    "ListDatasetsRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "Filter": DatasetFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": DominantLanguageDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEndpointsRequestRequestTypeDef = TypedDict(
+    "ListEndpointsRequestRequestTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestRequestTypeDef = TypedDict(
+    "ListEntityRecognizersRequestRequestTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEventsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EventsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListFlywheelsRequestRequestTypeDef = TypedDict(
+    "ListFlywheelsRequestRequestTypeDef",
+    {
+        "Filter": FlywheelFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+    },
+)
+_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "Filter": FlywheelIterationFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListFlywheelIterationHistoryRequestRequestTypeDef(
+    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
+    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
+):
+    pass
+
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
     {
         "DocumentClassifierName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -2984,52 +2991,255 @@
 
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
+DocumentClassifierInputDataConfigUnionTypeDef = Union[
+    DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
+]
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
+        "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
         "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+DocumentClassificationJobPropertiesTypeDef = TypedDict(
+    "DocumentClassificationJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "DocumentClassifierArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "EntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "EntityRecognizerArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+EventsDetectionJobPropertiesTypeDef = TypedDict(
+    "EventsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "TargetEventTypes": List[str],
+    },
+    total=False,
+)
+
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
+KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": PiiOutputDataConfigTypeDef,
+        "RedactionConfig": RedactionConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "Mode": PiiEntitiesDetectionModeType,
+    },
+    total=False,
+)
+
+SentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "SentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobPropertiesTypeDef = TypedDict(
+    "TopicsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "NumberOfTopics": int,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTaskConfigOutputTypeDef = TypedDict(
+    "_RequiredTaskConfigOutputTypeDef",
+    {
+        "LanguageCode": LanguageCodeType,
     },
 )
+_OptionalTaskConfigOutputTypeDef = TypedDict(
+    "_OptionalTaskConfigOutputTypeDef",
+    {
+        "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
+        "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
+    pass
 
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -3070,14 +3280,17 @@
 
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
+EntityRecognizerInputDataConfigUnionTypeDef = Union[
+    EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
+]
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3085,24 +3298,24 @@
     total=False,
 )
 
 DescribeFlywheelIterationResponseTypeDef = TypedDict(
     "DescribeFlywheelIterationResponseTypeDef",
     {
         "FlywheelIterationProperties": FlywheelIterationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFlywheelIterationHistoryResponseTypeDef = TypedDict(
     "ListFlywheelIterationHistoryResponseTypeDef",
     {
         "FlywheelIterationPropertiesList": List[FlywheelIterationPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "Id": str,
@@ -3124,15 +3337,15 @@
     total=False,
 )
 
 DetectSyntaxResponseTypeDef = TypedDict(
     "DetectSyntaxResponseTypeDef",
     {
         "SyntaxTokens": List[SyntaxTokenTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentEntityTypeDef = TypedDict(
     "TargetedSentimentEntityTypeDef",
     {
         "DescriptiveMentionIndex": List[int],
@@ -3146,212 +3359,231 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "DatasetName": str,
+        "InputDataConfig": DatasetInputDataConfigTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentClassificationJobsResponseTypeDef = TypedDict(
     "ListDocumentClassificationJobsResponseTypeDef",
     {
         "DocumentClassificationJobPropertiesList": List[DocumentClassificationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDominantLanguageDetectionJobResponseTypeDef = TypedDict(
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     {
         "DominantLanguageDetectionJobProperties": DominantLanguageDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDominantLanguageDetectionJobsResponseTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     {
         "DominantLanguageDetectionJobPropertiesList": List[
             DominantLanguageDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionJobResponseTypeDef",
     {
         "EntitiesDetectionJobProperties": EntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionJobsResponseTypeDef",
     {
         "EntitiesDetectionJobPropertiesList": List[EntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsDetectionJobResponseTypeDef = TypedDict(
     "DescribeEventsDetectionJobResponseTypeDef",
     {
         "EventsDetectionJobProperties": EventsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventsDetectionJobsResponseTypeDef = TypedDict(
     "ListEventsDetectionJobsResponseTypeDef",
     {
         "EventsDetectionJobPropertiesList": List[EventsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
     "DescribeKeyPhrasesDetectionJobResponseTypeDef",
     {
         "KeyPhrasesDetectionJobProperties": KeyPhrasesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeyPhrasesDetectionJobsResponseTypeDef = TypedDict(
     "ListKeyPhrasesDetectionJobsResponseTypeDef",
     {
         "KeyPhrasesDetectionJobPropertiesList": List[KeyPhrasesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePiiEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribePiiEntitiesDetectionJobResponseTypeDef",
     {
         "PiiEntitiesDetectionJobProperties": PiiEntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPiiEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     {
         "PiiEntitiesDetectionJobPropertiesList": List[PiiEntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeSentimentDetectionJobResponseTypeDef",
     {
         "SentimentDetectionJobProperties": SentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListSentimentDetectionJobsResponseTypeDef",
     {
         "SentimentDetectionJobPropertiesList": List[SentimentDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     {
         "TargetedSentimentDetectionJobProperties": TargetedSentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetedSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     {
         "TargetedSentimentDetectionJobPropertiesList": List[
             TargetedSentimentDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTopicsDetectionJobResponseTypeDef = TypedDict(
     "DescribeTopicsDetectionJobResponseTypeDef",
     {
         "TopicsDetectionJobProperties": TopicsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicsDetectionJobsResponseTypeDef = TypedDict(
     "ListTopicsDetectionJobsResponseTypeDef",
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
+FlywheelPropertiesTypeDef = TypedDict(
+    "FlywheelPropertiesTypeDef",
     {
         "FlywheelArn": str,
-        "DatasetName": str,
-        "InputDataConfig": DatasetInputDataConfigTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "Description": str,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "ActiveModelArn": str,
+        "DataAccessRoleArn": str,
+        "TaskConfig": TaskConfigOutputTypeDef,
+        "DataLakeS3Uri": str,
+        "DataSecurityConfig": DataSecurityConfigOutputTypeDef,
+        "Status": FlywheelStatusType,
+        "ModelType": ModelTypeType,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LatestFlywheelIteration": str,
     },
     total=False,
 )
 
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3370,49 +3602,31 @@
 )
 
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
-FlywheelPropertiesTypeDef = TypedDict(
-    "FlywheelPropertiesTypeDef",
-    {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "DataAccessRoleArn": str,
-        "TaskConfig": TaskConfigTypeDef,
-        "DataLakeS3Uri": str,
-        "DataSecurityConfig": DataSecurityConfigTypeDef,
-        "Status": FlywheelStatusType,
-        "ModelType": ModelTypeType,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LatestFlywheelIteration": str,
-    },
-    total=False,
-)
-
+TaskConfigUnionTypeDef = Union[TaskConfigTypeDef, TaskConfigOutputTypeDef]
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
+        "InputDataConfig": EntityRecognizerInputDataConfigOutputTypeDef,
         "RecognizerMetadata": EntityRecognizerMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
         "OutputDataConfig": EntityRecognizerOutputDataConfigTypeDef,
     },
     total=False,
@@ -3422,24 +3636,24 @@
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Blocks": List[BlockTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSyntaxResponseTypeDef = TypedDict(
     "BatchDetectSyntaxResponseTypeDef",
     {
         "ResultList": List[BatchDetectSyntaxItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentItemResultTypeDef = TypedDict(
     "BatchDetectTargetedSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -3448,61 +3662,61 @@
     total=False,
 )
 
 DetectTargetedSentimentResponseTypeDef = TypedDict(
     "DetectTargetedSentimentResponseTypeDef",
     {
         "Entities": List[TargetedSentimentEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectEntitiesResponseTypeDef = TypedDict(
     "BatchDetectEntitiesResponseTypeDef",
     {
         "ResultList": List[BatchDetectEntitiesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFlywheelResponseTypeDef = TypedDict(
     "DescribeFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlywheelResponseTypeDef = TypedDict(
     "UpdateFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityRecognizerResponseTypeDef = TypedDict(
     "DescribeEntityRecognizerResponseTypeDef",
     {
         "EntityRecognizerProperties": EntityRecognizerPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntityRecognizersResponseTypeDef = TypedDict(
     "ListEntityRecognizersResponseTypeDef",
     {
         "EntityRecognizerPropertiesList": List[EntityRecognizerPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentResponseTypeDef = TypedDict(
     "BatchDetectTargetedSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectTargetedSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/PKG-INFO` & `types-aiobotocore-comprehend-2.5.2.post1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-comprehend
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Comprehend 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore comprehend type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-comprehend"></a>
 
 # types-aiobotocore-comprehend
 
 [![PyPI - types-aiobotocore-comprehend](https://img.shields.io/pypi/v/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-comprehend?color=blue)](https://pypistats.org/packages/types-aiobotocore-comprehend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehend)](https://pepy.tech/project/types-aiobotocore-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Comprehend 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [types-aiobotocore-comprehend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -385,60 +352,59 @@
 )
 
 
 def check_value(value: AugmentedManifestsDocumentTypeFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_comprehend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_comprehend.type_defs import (
+    AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
+    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
+    BlobTypeDef,
     ChildBlockTypeDef,
     RelationshipsListItemTypeDef,
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
     WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
+    VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
-    DatasetFilterTypeDef,
+    TimestampTypeDef,
     DatasetPropertiesTypeDef,
     DeleteDocumentClassifierRequestRequestTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEntityRecognizerRequestRequestTypeDef,
     DeleteFlywheelRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
@@ -451,98 +417,91 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
+    DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
-    DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
-    DocumentClassifierFilterTypeDef,
+    DocumentReaderConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
-    DominantLanguageDetectionJobFilterTypeDef,
-    EndpointFilterTypeDef,
-    EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
     EntityRecognizerAnnotationsTypeDef,
     EntityRecognizerDocumentsTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
-    EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
-    EventsDetectionJobFilterTypeDef,
-    FlywheelFilterTypeDef,
-    FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    ImportModelResponseTypeDef,
-    KeyPhrasesDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
-    PiiEntitiesDetectionJobFilterTypeDef,
-    SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TargetedSentimentDetectionJobFilterTypeDef,
-    TopicsDetectionJobFilterTypeDef,
-    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    RedactionConfigTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    DetectDominantLanguageResponseTypeDef,
+    ImportModelResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
@@ -552,94 +511,125 @@
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
+    DataSecurityConfigOutputTypeDef,
+    VpcConfigUnionTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
-    ListDatasetsRequestRequestTypeDef,
+    DatasetFilterTypeDef,
+    DocumentClassificationJobFilterTypeDef,
+    DocumentClassifierFilterTypeDef,
+    DominantLanguageDetectionJobFilterTypeDef,
+    EndpointFilterTypeDef,
+    EntitiesDetectionJobFilterTypeDef,
+    EntityRecognizerFilterTypeDef,
+    EventsDetectionJobFilterTypeDef,
+    FlywheelFilterTypeDef,
+    FlywheelIterationFilterTypeDef,
+    KeyPhrasesDetectionJobFilterTypeDef,
+    PiiEntitiesDetectionJobFilterTypeDef,
+    SentimentDetectionJobFilterTypeDef,
+    TargetedSentimentDetectionJobFilterTypeDef,
+    TopicsDetectionJobFilterTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigOutputTypeDef,
+    DocumentReaderConfigUnionTypeDef,
+    InputDataConfigOutputTypeDef,
+    ListDocumentClassifierSummariesResponseTypeDef,
+    DocumentMetadataTypeDef,
+    EntityRecognitionConfigOutputTypeDef,
+    EntityRecognitionConfigTypeDef,
+    EntityRecognizerInputDataConfigOutputTypeDef,
+    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerMetadataEntityTypesListItemTypeDef,
+    ListEntityRecognizerSummariesResponseTypeDef,
+    FlywheelIterationPropertiesTypeDef,
+    ListFlywheelsResponseTypeDef,
+    GeometryTypeDef,
+    SyntaxTokenTypeDef,
+    RedactionConfigUnionTypeDef,
+    BatchDetectDominantLanguageResponseTypeDef,
+    BatchDetectKeyPhrasesResponseTypeDef,
+    BatchDetectSentimentResponseTypeDef,
+    TargetedSentimentMentionTypeDef,
+    EntityTypeDef,
+    StartDocumentClassificationJobRequestRequestTypeDef,
+    StartDominantLanguageDetectionJobRequestRequestTypeDef,
+    StartEntitiesDetectionJobRequestRequestTypeDef,
+    StartEventsDetectionJobRequestRequestTypeDef,
+    StartKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StartPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StartSentimentDetectionJobRequestRequestTypeDef,
+    StartTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StartTopicsDetectionJobRequestRequestTypeDef,
+    UpdateFlywheelRequestRequestTypeDef,
+    DataSecurityConfigUnionTypeDef,
+    DatasetInputDataConfigTypeDef,
+    ListDatasetsRequestRequestTypeDef,
     ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
     ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
-    ListDocumentClassifierSummariesResponseTypeDef,
-    DocumentMetadataTypeDef,
     ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
     ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
-    EntityRecognitionConfigTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
     ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
-    EntityRecognizerMetadataEntityTypesListItemTypeDef,
-    ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
-    FlywheelIterationPropertiesTypeDef,
-    ListFlywheelsResponseTypeDef,
-    GeometryTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
-    SyntaxTokenTypeDef,
-    BatchDetectDominantLanguageResponseTypeDef,
-    BatchDetectKeyPhrasesResponseTypeDef,
-    BatchDetectSentimentResponseTypeDef,
-    TargetedSentimentMentionTypeDef,
-    EntityTypeDef,
+    CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
+    DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
-    StartDocumentClassificationJobRequestRequestTypeDef,
-    StartDominantLanguageDetectionJobRequestRequestTypeDef,
-    StartEntitiesDetectionJobRequestRequestTypeDef,
-    StartEventsDetectionJobRequestRequestTypeDef,
-    StartKeyPhrasesDetectionJobRequestRequestTypeDef,
-    StartPiiEntitiesDetectionJobRequestRequestTypeDef,
-    StartSentimentDetectionJobRequestRequestTypeDef,
-    StartTargetedSentimentDetectionJobRequestRequestTypeDef,
-    StartTopicsDetectionJobRequestRequestTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
-    UpdateFlywheelRequestRequestTypeDef,
-    DatasetInputDataConfigTypeDef,
-    CreateDocumentClassifierRequestRequestTypeDef,
-    DocumentClassifierPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
+    TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -650,34 +640,32 @@
     ListPiiEntitiesDetectionJobsResponseTypeDef,
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
-    CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
+    CreateFlywheelRequestRequestTypeDef,
+    TaskConfigUnionTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemTypeDef:
+def get_value() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-comprehend-2.5.2/types_aiobotocore_comprehend.egg-info/SOURCES.txt` & `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*


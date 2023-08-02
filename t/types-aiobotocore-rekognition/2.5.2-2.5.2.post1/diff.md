# Comparing `tmp/types-aiobotocore-rekognition-2.5.2.tar.gz` & `tmp/types-aiobotocore-rekognition-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rekognition-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-rekognition-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-rekognition-2.5.2.tar` & `types-aiobotocore-rekognition-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.334762 types-aiobotocore-rekognition-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26915 2023-07-08 01:44:11.326762 types-aiobotocore-rekognition-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25334 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.334762 types-aiobotocore-rekognition-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.326762 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60517 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60425 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-08 01:39:09.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-08 01:39:09.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97151 2023-07-08 01:39:13.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-07-08 01:39:12.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-08 01:39:08.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.326762 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26915 2023-07-08 01:44:11.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-08 01:44:11.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:44:11.000000 types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25646 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.385483 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60562 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60470 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-02 14:47:47.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98991 2023-08-02 14:47:48.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98870 2023-08-02 14:47:47.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rekognition-2.5.2/LICENSE` & `types-aiobotocore-rekognition-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/PKG-INFO` & `types-aiobotocore-rekognition-2.5.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rekognition
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Rekognition 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Rekognition 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore rekognition type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore rekognition type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rekognition"></a>
 
 # types-aiobotocore-rekognition
 
 [![PyPI - types-aiobotocore-rekognition](https://img.shields.io/pypi/v/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rekognition?color=blue)](https://pypistats.org/packages/types-aiobotocore-rekognition)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Rekognition 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [types-aiobotocore-rekognition docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -416,79 +415,69 @@
 )
 
 
 def check_value(value: AttributeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_rekognition.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
+    ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
     BoundingBoxTypeDef,
     S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BlobTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
+    ConnectedHomeSettingsOutputTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
-    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
     LivenessOutputConfigTypeDef,
-    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
-    CreateStreamProcessorResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
-    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
-    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
-    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
@@ -526,100 +515,113 @@
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    PaginatorConfigTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
-    PutProjectPolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
+    StartShotDetectionFilterTypeDef,
+    StreamProcessingStopSelectorTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    CopyProjectVersionResponseTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    DeleteCollectionResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteProjectVersionResponseTypeDef,
+    DescribeCollectionResponseTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
-    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
-    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
     GroundTruthManifestTypeDef,
-    ImageTypeDef,
     SummaryTypeDef,
     VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
+    DatasetChangesTypeDef,
+    ImageTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
     LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
+    RegionOfInterestOutputTypeDef,
     RegionOfInterestTypeDef,
     HumanLoopConfigTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
@@ -627,29 +629,30 @@
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
     AssetTypeDef,
     DatasetSourceTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     CompareFacesRequestRequestTypeDef,
     DetectCustomLabelsRequestRequestTypeDef,
     DetectFacesRequestRequestTypeDef,
     DetectProtectiveEquipmentRequestRequestTypeDef,
     IndexFacesRequestRequestTypeDef,
     RecognizeCelebritiesRequestRequestTypeDef,
     SearchFacesByImageRequestRequestTypeDef,
     SearchUsersByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
@@ -662,28 +665,30 @@
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
+    RegionOfInterestUnionTypeDef,
     StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
-    CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    TestingDataOutputTypeDef,
     TestingDataTypeDef,
+    TrainingDataOutputTypeDef,
     TrainingDataTypeDef,
     ValidationDataTypeDef,
     CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
@@ -695,30 +700,34 @@
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
+    CreateStreamProcessorRequestRequestTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    TestingDataUnionTypeDef,
     CreateProjectVersionRequestRequestTypeDef,
+    TrainingDataUnionTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
-def get_structure() -> AgeRangeTypeDef:
+def get_value() -> AgeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rekognition-2.5.2/README.md` & `types-aiobotocore-rekognition-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-rekognition"></a>
 
 # types-aiobotocore-rekognition
 
 [![PyPI - types-aiobotocore-rekognition](https://img.shields.io/pypi/v/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rekognition?color=blue)](https://pypistats.org/packages/types-aiobotocore-rekognition)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Rekognition 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [types-aiobotocore-rekognition docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -383,79 +383,69 @@
 )
 
 
 def check_value(value: AttributeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_rekognition.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
+    ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
     BoundingBoxTypeDef,
     S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BlobTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
+    ConnectedHomeSettingsOutputTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
-    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
     LivenessOutputConfigTypeDef,
-    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
-    CreateStreamProcessorResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
-    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
-    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
-    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
@@ -493,100 +483,113 @@
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    PaginatorConfigTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
-    PutProjectPolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
+    StartShotDetectionFilterTypeDef,
+    StreamProcessingStopSelectorTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    CopyProjectVersionResponseTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    DeleteCollectionResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteProjectVersionResponseTypeDef,
+    DescribeCollectionResponseTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
-    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
-    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
     GroundTruthManifestTypeDef,
-    ImageTypeDef,
     SummaryTypeDef,
     VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
+    DatasetChangesTypeDef,
+    ImageTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
     LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
+    RegionOfInterestOutputTypeDef,
     RegionOfInterestTypeDef,
     HumanLoopConfigTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
@@ -594,29 +597,30 @@
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
     AssetTypeDef,
     DatasetSourceTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     CompareFacesRequestRequestTypeDef,
     DetectCustomLabelsRequestRequestTypeDef,
     DetectFacesRequestRequestTypeDef,
     DetectProtectiveEquipmentRequestRequestTypeDef,
     IndexFacesRequestRequestTypeDef,
     RecognizeCelebritiesRequestRequestTypeDef,
     SearchFacesByImageRequestRequestTypeDef,
     SearchUsersByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
@@ -629,28 +633,30 @@
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
+    RegionOfInterestUnionTypeDef,
     StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
-    CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    TestingDataOutputTypeDef,
     TestingDataTypeDef,
+    TrainingDataOutputTypeDef,
     TrainingDataTypeDef,
     ValidationDataTypeDef,
     CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
@@ -662,30 +668,34 @@
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
+    CreateStreamProcessorRequestRequestTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    TestingDataUnionTypeDef,
     CreateProjectVersionRequestRequestTypeDef,
+    TrainingDataUnionTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
-def get_structure() -> AgeRangeTypeDef:
+def get_value() -> AgeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rekognition-2.5.2/setup.py` & `types-aiobotocore-rekognition-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rekognition",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Rekognition 2.5.2 service generated with"
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
-    keywords="aiobotocore rekognition type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore rekognition type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rekognition": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/"
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/__init__.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/__init__.pyi` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/__main__.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Rekognition 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Rekognition 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/client.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestUnionTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -127,38 +127,35 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
+    TestingDataUnionTypeDef,
+    TrainingDataUnionTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RekognitionClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     HumanLoopQuotaExceededException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     ImageTooLargeException: Type[BotocoreClientError]
@@ -176,15 +173,14 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     SessionNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     VideoTooLargeException: Type[BotocoreClientError]
 
-
 class RekognitionClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
     """
 
     meta: ClientMeta
@@ -193,15 +189,14 @@
     def exceptions(self) -> Exceptions:
         """
         RekognitionClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#exceptions)
         """
-
     async def associate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
         UserMatchThreshold: float = ...,
@@ -209,31 +204,28 @@
     ) -> AssociateFacesResponseTypeDef:
         """
         Associates one or more faces with an existing UserID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.associate_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#associate_faces)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#close)
         """
-
     async def compare_faces(
         self,
         *,
         SourceImage: ImageTypeDef,
         TargetImage: ImageTypeDef,
         SimilarityThreshold: float = ...,
         QualityFilter: QualityFilterType = ...
@@ -241,15 +233,14 @@
         """
         Compares a face in the *source* input image with each of the 100 largest faces
         detected in the *target* input image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.compare_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#compare_faces)
         """
-
     async def copy_project_version(
         self,
         *,
         SourceProjectArn: str,
         SourceProjectVersionArn: str,
         DestinationProjectArn: str,
         VersionName: str,
@@ -260,199 +251,181 @@
         """
         Copies a version of an Amazon Rekognition Custom Labels model from a source
         project to a destination project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.copy_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#copy_project_version)
         """
-
     async def create_collection(
         self, *, CollectionId: str, Tags: Mapping[str, str] = ...
     ) -> CreateCollectionResponseTypeDef:
         """
         Creates a collection in an AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_collection)
         """
-
     async def create_dataset(
         self,
         *,
         DatasetType: DatasetTypeType,
         ProjectArn: str,
         DatasetSource: DatasetSourceTypeDef = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_dataset)
         """
-
     async def create_face_liveness_session(
         self,
         *,
         KmsKeyId: str = ...,
         Settings: CreateFaceLivenessSessionRequestSettingsTypeDef = ...,
         ClientRequestToken: str = ...
     ) -> CreateFaceLivenessSessionResponseTypeDef:
         """
         This API operation initiates a Face Liveness session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_face_liveness_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_face_liveness_session)
         """
-
     async def create_project(self, *, ProjectName: str) -> CreateProjectResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_project)
         """
-
     async def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataTypeDef = ...,
-        TestingData: TestingDataTypeDef = ...,
+        TrainingData: TrainingDataUnionTypeDef = ...,
+        TestingData: TestingDataUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_project_version)
         """
-
     async def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsTypeDef,
+        Settings: StreamProcessorSettingsUnionTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_stream_processor)
         """
-
     async def create_user(
         self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a new User within a collection specified by `CollectionId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_user)
         """
-
     async def delete_collection(self, *, CollectionId: str) -> DeleteCollectionResponseTypeDef:
         """
         Deletes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_collection)
         """
-
     async def delete_dataset(self, *, DatasetArn: str) -> Dict[str, Any]:
         """
         Deletes an existing Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_dataset)
         """
-
     async def delete_faces(
         self, *, CollectionId: str, FaceIds: Sequence[str]
     ) -> DeleteFacesResponseTypeDef:
         """
         Deletes faces from a collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_faces)
         """
-
     async def delete_project(self, *, ProjectArn: str) -> DeleteProjectResponseTypeDef:
         """
         Deletes an Amazon Rekognition Custom Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_project)
         """
-
     async def delete_project_policy(
         self, *, ProjectArn: str, PolicyName: str, PolicyRevisionId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes an existing project policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_project_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_project_policy)
         """
-
     async def delete_project_version(
         self, *, ProjectVersionArn: str
     ) -> DeleteProjectVersionResponseTypeDef:
         """
         Deletes an Amazon Rekognition Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_project_version)
         """
-
     async def delete_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes the stream processor identified by `Name`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_stream_processor)
         """
-
     async def delete_user(
         self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified UserID within the collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_user)
         """
-
     async def describe_collection(self, *, CollectionId: str) -> DescribeCollectionResponseTypeDef:
         """
         Describes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_collection)
         """
-
     async def describe_dataset(self, *, DatasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Describes an Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_dataset)
         """
-
     async def describe_project_versions(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -460,35 +433,32 @@
         """
         Lists and describes the versions of a model in an Amazon Rekognition Custom
         Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_project_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_project_versions)
         """
-
     async def describe_projects(
         self, *, NextToken: str = ..., MaxResults: int = ..., ProjectNames: Sequence[str] = ...
     ) -> DescribeProjectsResponseTypeDef:
         """
         Gets information about your Amazon Rekognition Custom Labels projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_projects)
         """
-
     async def describe_stream_processor(
         self, *, Name: str
     ) -> DescribeStreamProcessorResponseTypeDef:
         """
         Provides information about a stream processor created by  CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_stream_processor)
         """
-
     async def detect_custom_labels(
         self,
         *,
         ProjectVersionArn: str,
         Image: ImageTypeDef,
         MaxResults: int = ...,
         MinConfidence: float = ...
@@ -496,25 +466,23 @@
         """
         Detects custom labels in a supplied image by using an Amazon Rekognition Custom
         Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_custom_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_custom_labels)
         """
-
     async def detect_faces(
         self, *, Image: ImageTypeDef, Attributes: Sequence[AttributeType] = ...
     ) -> DetectFacesResponseTypeDef:
         """
         Detects faces within an image that is provided as input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_faces)
         """
-
     async def detect_labels(
         self,
         *,
         Image: ImageTypeDef,
         MaxLabels: int = ...,
         MinConfidence: float = ...,
         Features: Sequence[DetectLabelsFeatureNameType] = ...,
@@ -523,52 +491,48 @@
         """
         Detects instances of real-world entities within an image (JPEG or PNG) provided
         as input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_labels)
         """
-
     async def detect_moderation_labels(
         self,
         *,
         Image: ImageTypeDef,
         MinConfidence: float = ...,
         HumanLoopConfig: HumanLoopConfigTypeDef = ...
     ) -> DetectModerationLabelsResponseTypeDef:
         """
         Detects unsafe content in a specified JPEG or PNG format image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_moderation_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_moderation_labels)
         """
-
     async def detect_protective_equipment(
         self,
         *,
         Image: ImageTypeDef,
         SummarizationAttributes: ProtectiveEquipmentSummarizationAttributesTypeDef = ...
     ) -> DetectProtectiveEquipmentResponseTypeDef:
         """
         Detects Personal Protective Equipment (PPE) worn by people detected in an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_protective_equipment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_protective_equipment)
         """
-
     async def detect_text(
         self, *, Image: ImageTypeDef, Filters: DetectTextFiltersTypeDef = ...
     ) -> DetectTextResponseTypeDef:
         """
         Detects text in the input image and converts it into machine-readable text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_text)
         """
-
     async def disassociate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
         ClientRequestToken: str = ...
@@ -576,49 +540,45 @@
         """
         Removes the association between a `Face` supplied in an array of `FaceIds` and
         the User.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.disassociate_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#disassociate_faces)
         """
-
     async def distribute_dataset_entries(
         self, *, Datasets: Sequence[DistributeDatasetTypeDef]
     ) -> Dict[str, Any]:
         """
         Distributes the entries (images) in a training dataset across the training
         dataset and the test dataset for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.distribute_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#distribute_dataset_entries)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#generate_presigned_url)
         """
-
     async def get_celebrity_info(self, *, Id: str) -> GetCelebrityInfoResponseTypeDef:
         """
         Gets the name and additional information about a celebrity based on their Amazon
         Rekognition ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_info)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_celebrity_info)
         """
-
     async def get_celebrity_recognition(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: CelebrityRecognitionSortByType = ...
@@ -626,15 +586,14 @@
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
         started by  StartCelebrityRecognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_celebrity_recognition)
         """
-
     async def get_content_moderation(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ContentModerationSortByType = ...,
@@ -643,36 +602,33 @@
         """
         Gets the inappropriate, unwanted, or offensive content analysis results for a
         Amazon Rekognition Video analysis started by  StartContentModeration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_content_moderation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_content_moderation)
         """
-
     async def get_face_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetFaceDetectionResponseTypeDef:
         """
         Gets face detection results for a Amazon Rekognition Video analysis started by
         StartFaceDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_face_detection)
         """
-
     async def get_face_liveness_session_results(
         self, *, SessionId: str
     ) -> GetFaceLivenessSessionResultsResponseTypeDef:
         """
         Retrieves the results of a specific Face Liveness session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_liveness_session_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_face_liveness_session_results)
         """
-
     async def get_face_search(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: FaceSearchSortByType = ...
@@ -680,15 +636,14 @@
         """
         Gets the face search results for Amazon Rekognition Video face search started by
         StartFaceSearch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_face_search)
         """
-
     async def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: LabelDetectionSortByType = ...,
@@ -697,15 +652,14 @@
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
         by  StartLabelDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_label_detection)
         """
-
     async def get_person_tracking(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: PersonTrackingSortByType = ...
@@ -713,37 +667,34 @@
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started by
         StartPersonTracking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_person_tracking)
         """
-
     async def get_segment_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetSegmentDetectionResponseTypeDef:
         """
         Gets the segment detection results of a Amazon Rekognition Video analysis
         started by  StartSegmentDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_segment_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_segment_detection)
         """
-
     async def get_text_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetTextDetectionResponseTypeDef:
         """
         Gets the text detection results of a Amazon Rekognition Video analysis started
         by  StartTextDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_text_detection)
         """
-
     async def index_faces(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         ExternalImageId: str = ...,
         DetectionAttributes: Sequence[AttributeType] = ...,
@@ -752,25 +703,23 @@
     ) -> IndexFacesResponseTypeDef:
         """
         Detects faces in the input image and adds them to the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.index_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#index_faces)
         """
-
     async def list_collections(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCollectionsResponseTypeDef:
         """
         Returns list of collection IDs in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_collections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_collections)
         """
-
     async def list_dataset_entries(
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
@@ -780,25 +729,23 @@
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         Lists the entries (images) within a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_dataset_entries)
         """
-
     async def list_dataset_labels(
         self, *, DatasetArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDatasetLabelsResponseTypeDef:
         """
         Lists the labels in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_dataset_labels)
         """
-
     async def list_faces(
         self,
         *,
         CollectionId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         UserId: str = ...,
@@ -806,78 +753,71 @@
     ) -> ListFacesResponseTypeDef:
         """
         Returns metadata for faces in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_faces)
         """
-
     async def list_project_policies(
         self, *, ProjectArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProjectPoliciesResponseTypeDef:
         """
         Gets a list of the project policies attached to a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_project_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_project_policies)
         """
-
     async def list_stream_processors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListStreamProcessorsResponseTypeDef:
         """
         Gets a list of stream processors that you have created with
         CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_stream_processors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_stream_processors)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags in an Amazon Rekognition collection, stream processor, or
         Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_tags_for_resource)
         """
-
     async def list_users(
         self, *, CollectionId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListUsersResponseTypeDef:
         """
         Returns metadata of the User such as `UserID` in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_users)
         """
-
     async def put_project_policy(
         self, *, ProjectArn: str, PolicyName: str, PolicyDocument: str, PolicyRevisionId: str = ...
     ) -> PutProjectPolicyResponseTypeDef:
         """
         Attaches a project policy to a Amazon Rekognition Custom Labels project in a
         trusting AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.put_project_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#put_project_policy)
         """
-
     async def recognize_celebrities(
         self, *, Image: ImageTypeDef
     ) -> RecognizeCelebritiesResponseTypeDef:
         """
         Returns an array of celebrities recognized in the input image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.recognize_celebrities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#recognize_celebrities)
         """
-
     async def search_faces(
         self,
         *,
         CollectionId: str,
         FaceId: str,
         MaxFaces: int = ...,
         FaceMatchThreshold: float = ...
@@ -885,15 +825,14 @@
         """
         For a given input face ID, searches for matching faces in the collection the
         face belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_faces)
         """
-
     async def search_faces_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         MaxFaces: int = ...,
         FaceMatchThreshold: float = ...,
@@ -902,15 +841,14 @@
         """
         For a given input image, first detects the largest face in the image, and then
         searches the specified collection for matching faces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces_by_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_faces_by_image)
         """
-
     async def search_users(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceId: str = ...,
         UserMatchThreshold: float = ...,
@@ -918,15 +856,14 @@
     ) -> SearchUsersResponseTypeDef:
         """
         Searches for UserIDs within a collection based on a `FaceId` or `UserId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users)
         """
-
     async def search_users_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         UserMatchThreshold: float = ...,
         MaxUsers: int = ...,
@@ -934,30 +871,28 @@
     ) -> SearchUsersByImageResponseTypeDef:
         """
         Searches for UserIDs using a supplied image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users_by_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users_by_image)
         """
-
     async def start_celebrity_recognition(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...
     ) -> StartCelebrityRecognitionResponseTypeDef:
         """
         Starts asynchronous recognition of celebrities in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_celebrity_recognition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_celebrity_recognition)
         """
-
     async def start_content_moderation(
         self,
         *,
         Video: VideoTypeDef,
         MinConfidence: float = ...,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
@@ -966,15 +901,14 @@
         """
         Starts asynchronous detection of inappropriate, unwanted, or offensive content
         in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_content_moderation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_content_moderation)
         """
-
     async def start_face_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         FaceAttributes: FaceAttributesType = ...,
@@ -982,15 +916,14 @@
     ) -> StartFaceDetectionResponseTypeDef:
         """
         Starts asynchronous detection of faces in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_face_detection)
         """
-
     async def start_face_search(
         self,
         *,
         Video: VideoTypeDef,
         CollectionId: str,
         ClientRequestToken: str = ...,
         FaceMatchThreshold: float = ...,
@@ -1000,15 +933,14 @@
         """
         Starts the asynchronous search for faces in a collection that match the faces of
         persons detected in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_face_search)
         """
-
     async def start_label_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
@@ -1018,40 +950,37 @@
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_label_detection)
         """
-
     async def start_person_tracking(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...
     ) -> StartPersonTrackingResponseTypeDef:
         """
         Starts the asynchronous tracking of a person's path in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_person_tracking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_person_tracking)
         """
-
     async def start_project_version(
         self, *, ProjectVersionArn: str, MinInferenceUnits: int, MaxInferenceUnits: int = ...
     ) -> StartProjectVersionResponseTypeDef:
         """
         Starts the running of the version of a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_project_version)
         """
-
     async def start_segment_detection(
         self,
         *,
         Video: VideoTypeDef,
         SegmentTypes: Sequence[SegmentTypeType],
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
@@ -1060,29 +989,27 @@
     ) -> StartSegmentDetectionResponseTypeDef:
         """
         Starts asynchronous detection of segment detection in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_segment_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_segment_detection)
         """
-
     async def start_stream_processor(
         self,
         *,
         Name: str,
         StartSelector: StreamProcessingStartSelectorTypeDef = ...,
         StopSelector: StreamProcessingStopSelectorTypeDef = ...
     ) -> StartStreamProcessorResponseTypeDef:
         """
         Starts processing a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_stream_processor)
         """
-
     async def start_text_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
@@ -1090,176 +1017,157 @@
     ) -> StartTextDetectionResponseTypeDef:
         """
         Starts asynchronous detection of text in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_text_detection)
         """
-
     async def stop_project_version(
         self, *, ProjectVersionArn: str
     ) -> StopProjectVersionResponseTypeDef:
         """
         Stops a running model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#stop_project_version)
         """
-
     async def stop_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops a running stream processor that was created by  CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#stop_stream_processor)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more key-value tags to an Amazon Rekognition collection, stream
         processor, or Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from an Amazon Rekognition collection, stream
         processor, or Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#untag_resource)
         """
-
     async def update_dataset_entries(
         self, *, DatasetArn: str, Changes: DatasetChangesTypeDef
     ) -> Dict[str, Any]:
         """
         Adds or updates one or more entries (images) in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_dataset_entries)
         """
-
     async def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_stream_processor)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_project_versions"]
     ) -> DescribeProjectVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_projects"]
     ) -> DescribeProjectsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_collections"]
     ) -> ListCollectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dataset_entries"]
     ) -> ListDatasetEntriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dataset_labels"]
     ) -> ListDatasetLabelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_faces"]) -> ListFacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_project_policies"]
     ) -> ListProjectPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_stream_processors"]
     ) -> ListStreamProcessorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_users"]) -> ListUsersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["project_version_running"]
     ) -> ProjectVersionRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["project_version_training_completed"]
     ) -> ProjectVersionTrainingCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "RekognitionClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
         """
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/client.pyi` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestUnionTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -127,35 +127,38 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
+    TestingDataUnionTypeDef,
+    TrainingDataUnionTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("RekognitionClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     HumanLoopQuotaExceededException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     ImageTooLargeException: Type[BotocoreClientError]
@@ -173,14 +176,15 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     SessionNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     VideoTooLargeException: Type[BotocoreClientError]
 
+
 class RekognitionClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
     """
 
     meta: ClientMeta
@@ -189,14 +193,15 @@
     def exceptions(self) -> Exceptions:
         """
         RekognitionClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#exceptions)
         """
+
     async def associate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
         UserMatchThreshold: float = ...,
@@ -204,28 +209,31 @@
     ) -> AssociateFacesResponseTypeDef:
         """
         Associates one or more faces with an existing UserID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.associate_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#associate_faces)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#close)
         """
+
     async def compare_faces(
         self,
         *,
         SourceImage: ImageTypeDef,
         TargetImage: ImageTypeDef,
         SimilarityThreshold: float = ...,
         QualityFilter: QualityFilterType = ...
@@ -233,14 +241,15 @@
         """
         Compares a face in the *source* input image with each of the 100 largest faces
         detected in the *target* input image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.compare_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#compare_faces)
         """
+
     async def copy_project_version(
         self,
         *,
         SourceProjectArn: str,
         SourceProjectVersionArn: str,
         DestinationProjectArn: str,
         VersionName: str,
@@ -251,181 +260,199 @@
         """
         Copies a version of an Amazon Rekognition Custom Labels model from a source
         project to a destination project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.copy_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#copy_project_version)
         """
+
     async def create_collection(
         self, *, CollectionId: str, Tags: Mapping[str, str] = ...
     ) -> CreateCollectionResponseTypeDef:
         """
         Creates a collection in an AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_collection)
         """
+
     async def create_dataset(
         self,
         *,
         DatasetType: DatasetTypeType,
         ProjectArn: str,
         DatasetSource: DatasetSourceTypeDef = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_dataset)
         """
+
     async def create_face_liveness_session(
         self,
         *,
         KmsKeyId: str = ...,
         Settings: CreateFaceLivenessSessionRequestSettingsTypeDef = ...,
         ClientRequestToken: str = ...
     ) -> CreateFaceLivenessSessionResponseTypeDef:
         """
         This API operation initiates a Face Liveness session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_face_liveness_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_face_liveness_session)
         """
+
     async def create_project(self, *, ProjectName: str) -> CreateProjectResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_project)
         """
+
     async def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataTypeDef = ...,
-        TestingData: TestingDataTypeDef = ...,
+        TrainingData: TrainingDataUnionTypeDef = ...,
+        TestingData: TestingDataUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_project_version)
         """
+
     async def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsTypeDef,
+        Settings: StreamProcessorSettingsUnionTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_stream_processor)
         """
+
     async def create_user(
         self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a new User within a collection specified by `CollectionId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_user)
         """
+
     async def delete_collection(self, *, CollectionId: str) -> DeleteCollectionResponseTypeDef:
         """
         Deletes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_collection)
         """
+
     async def delete_dataset(self, *, DatasetArn: str) -> Dict[str, Any]:
         """
         Deletes an existing Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_dataset)
         """
+
     async def delete_faces(
         self, *, CollectionId: str, FaceIds: Sequence[str]
     ) -> DeleteFacesResponseTypeDef:
         """
         Deletes faces from a collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_faces)
         """
+
     async def delete_project(self, *, ProjectArn: str) -> DeleteProjectResponseTypeDef:
         """
         Deletes an Amazon Rekognition Custom Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_project)
         """
+
     async def delete_project_policy(
         self, *, ProjectArn: str, PolicyName: str, PolicyRevisionId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes an existing project policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_project_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_project_policy)
         """
+
     async def delete_project_version(
         self, *, ProjectVersionArn: str
     ) -> DeleteProjectVersionResponseTypeDef:
         """
         Deletes an Amazon Rekognition Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_project_version)
         """
+
     async def delete_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes the stream processor identified by `Name`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_stream_processor)
         """
+
     async def delete_user(
         self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified UserID within the collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#delete_user)
         """
+
     async def describe_collection(self, *, CollectionId: str) -> DescribeCollectionResponseTypeDef:
         """
         Describes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_collection)
         """
+
     async def describe_dataset(self, *, DatasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Describes an Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_dataset)
         """
+
     async def describe_project_versions(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -433,32 +460,35 @@
         """
         Lists and describes the versions of a model in an Amazon Rekognition Custom
         Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_project_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_project_versions)
         """
+
     async def describe_projects(
         self, *, NextToken: str = ..., MaxResults: int = ..., ProjectNames: Sequence[str] = ...
     ) -> DescribeProjectsResponseTypeDef:
         """
         Gets information about your Amazon Rekognition Custom Labels projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_projects)
         """
+
     async def describe_stream_processor(
         self, *, Name: str
     ) -> DescribeStreamProcessorResponseTypeDef:
         """
         Provides information about a stream processor created by  CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_stream_processor)
         """
+
     async def detect_custom_labels(
         self,
         *,
         ProjectVersionArn: str,
         Image: ImageTypeDef,
         MaxResults: int = ...,
         MinConfidence: float = ...
@@ -466,23 +496,25 @@
         """
         Detects custom labels in a supplied image by using an Amazon Rekognition Custom
         Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_custom_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_custom_labels)
         """
+
     async def detect_faces(
         self, *, Image: ImageTypeDef, Attributes: Sequence[AttributeType] = ...
     ) -> DetectFacesResponseTypeDef:
         """
         Detects faces within an image that is provided as input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_faces)
         """
+
     async def detect_labels(
         self,
         *,
         Image: ImageTypeDef,
         MaxLabels: int = ...,
         MinConfidence: float = ...,
         Features: Sequence[DetectLabelsFeatureNameType] = ...,
@@ -491,48 +523,52 @@
         """
         Detects instances of real-world entities within an image (JPEG or PNG) provided
         as input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_labels)
         """
+
     async def detect_moderation_labels(
         self,
         *,
         Image: ImageTypeDef,
         MinConfidence: float = ...,
         HumanLoopConfig: HumanLoopConfigTypeDef = ...
     ) -> DetectModerationLabelsResponseTypeDef:
         """
         Detects unsafe content in a specified JPEG or PNG format image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_moderation_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_moderation_labels)
         """
+
     async def detect_protective_equipment(
         self,
         *,
         Image: ImageTypeDef,
         SummarizationAttributes: ProtectiveEquipmentSummarizationAttributesTypeDef = ...
     ) -> DetectProtectiveEquipmentResponseTypeDef:
         """
         Detects Personal Protective Equipment (PPE) worn by people detected in an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_protective_equipment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_protective_equipment)
         """
+
     async def detect_text(
         self, *, Image: ImageTypeDef, Filters: DetectTextFiltersTypeDef = ...
     ) -> DetectTextResponseTypeDef:
         """
         Detects text in the input image and converts it into machine-readable text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_text)
         """
+
     async def disassociate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
         ClientRequestToken: str = ...
@@ -540,45 +576,49 @@
         """
         Removes the association between a `Face` supplied in an array of `FaceIds` and
         the User.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.disassociate_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#disassociate_faces)
         """
+
     async def distribute_dataset_entries(
         self, *, Datasets: Sequence[DistributeDatasetTypeDef]
     ) -> Dict[str, Any]:
         """
         Distributes the entries (images) in a training dataset across the training
         dataset and the test dataset for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.distribute_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#distribute_dataset_entries)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#generate_presigned_url)
         """
+
     async def get_celebrity_info(self, *, Id: str) -> GetCelebrityInfoResponseTypeDef:
         """
         Gets the name and additional information about a celebrity based on their Amazon
         Rekognition ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_info)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_celebrity_info)
         """
+
     async def get_celebrity_recognition(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: CelebrityRecognitionSortByType = ...
@@ -586,14 +626,15 @@
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
         started by  StartCelebrityRecognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_celebrity_recognition)
         """
+
     async def get_content_moderation(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ContentModerationSortByType = ...,
@@ -602,33 +643,36 @@
         """
         Gets the inappropriate, unwanted, or offensive content analysis results for a
         Amazon Rekognition Video analysis started by  StartContentModeration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_content_moderation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_content_moderation)
         """
+
     async def get_face_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetFaceDetectionResponseTypeDef:
         """
         Gets face detection results for a Amazon Rekognition Video analysis started by
         StartFaceDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_face_detection)
         """
+
     async def get_face_liveness_session_results(
         self, *, SessionId: str
     ) -> GetFaceLivenessSessionResultsResponseTypeDef:
         """
         Retrieves the results of a specific Face Liveness session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_liveness_session_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_face_liveness_session_results)
         """
+
     async def get_face_search(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: FaceSearchSortByType = ...
@@ -636,14 +680,15 @@
         """
         Gets the face search results for Amazon Rekognition Video face search started by
         StartFaceSearch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_face_search)
         """
+
     async def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: LabelDetectionSortByType = ...,
@@ -652,14 +697,15 @@
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
         by  StartLabelDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_label_detection)
         """
+
     async def get_person_tracking(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: PersonTrackingSortByType = ...
@@ -667,34 +713,37 @@
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started by
         StartPersonTracking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_person_tracking)
         """
+
     async def get_segment_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetSegmentDetectionResponseTypeDef:
         """
         Gets the segment detection results of a Amazon Rekognition Video analysis
         started by  StartSegmentDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_segment_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_segment_detection)
         """
+
     async def get_text_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetTextDetectionResponseTypeDef:
         """
         Gets the text detection results of a Amazon Rekognition Video analysis started
         by  StartTextDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_text_detection)
         """
+
     async def index_faces(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         ExternalImageId: str = ...,
         DetectionAttributes: Sequence[AttributeType] = ...,
@@ -703,23 +752,25 @@
     ) -> IndexFacesResponseTypeDef:
         """
         Detects faces in the input image and adds them to the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.index_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#index_faces)
         """
+
     async def list_collections(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCollectionsResponseTypeDef:
         """
         Returns list of collection IDs in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_collections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_collections)
         """
+
     async def list_dataset_entries(
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
@@ -729,23 +780,25 @@
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         Lists the entries (images) within a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_dataset_entries)
         """
+
     async def list_dataset_labels(
         self, *, DatasetArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDatasetLabelsResponseTypeDef:
         """
         Lists the labels in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_dataset_labels)
         """
+
     async def list_faces(
         self,
         *,
         CollectionId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         UserId: str = ...,
@@ -753,71 +806,78 @@
     ) -> ListFacesResponseTypeDef:
         """
         Returns metadata for faces in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_faces)
         """
+
     async def list_project_policies(
         self, *, ProjectArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProjectPoliciesResponseTypeDef:
         """
         Gets a list of the project policies attached to a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_project_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_project_policies)
         """
+
     async def list_stream_processors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListStreamProcessorsResponseTypeDef:
         """
         Gets a list of stream processors that you have created with
         CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_stream_processors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_stream_processors)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags in an Amazon Rekognition collection, stream processor, or
         Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_tags_for_resource)
         """
+
     async def list_users(
         self, *, CollectionId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListUsersResponseTypeDef:
         """
         Returns metadata of the User such as `UserID` in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_users)
         """
+
     async def put_project_policy(
         self, *, ProjectArn: str, PolicyName: str, PolicyDocument: str, PolicyRevisionId: str = ...
     ) -> PutProjectPolicyResponseTypeDef:
         """
         Attaches a project policy to a Amazon Rekognition Custom Labels project in a
         trusting AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.put_project_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#put_project_policy)
         """
+
     async def recognize_celebrities(
         self, *, Image: ImageTypeDef
     ) -> RecognizeCelebritiesResponseTypeDef:
         """
         Returns an array of celebrities recognized in the input image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.recognize_celebrities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#recognize_celebrities)
         """
+
     async def search_faces(
         self,
         *,
         CollectionId: str,
         FaceId: str,
         MaxFaces: int = ...,
         FaceMatchThreshold: float = ...
@@ -825,14 +885,15 @@
         """
         For a given input face ID, searches for matching faces in the collection the
         face belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_faces)
         """
+
     async def search_faces_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         MaxFaces: int = ...,
         FaceMatchThreshold: float = ...,
@@ -841,14 +902,15 @@
         """
         For a given input image, first detects the largest face in the image, and then
         searches the specified collection for matching faces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces_by_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_faces_by_image)
         """
+
     async def search_users(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceId: str = ...,
         UserMatchThreshold: float = ...,
@@ -856,14 +918,15 @@
     ) -> SearchUsersResponseTypeDef:
         """
         Searches for UserIDs within a collection based on a `FaceId` or `UserId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users)
         """
+
     async def search_users_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         UserMatchThreshold: float = ...,
         MaxUsers: int = ...,
@@ -871,28 +934,30 @@
     ) -> SearchUsersByImageResponseTypeDef:
         """
         Searches for UserIDs using a supplied image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users_by_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users_by_image)
         """
+
     async def start_celebrity_recognition(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...
     ) -> StartCelebrityRecognitionResponseTypeDef:
         """
         Starts asynchronous recognition of celebrities in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_celebrity_recognition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_celebrity_recognition)
         """
+
     async def start_content_moderation(
         self,
         *,
         Video: VideoTypeDef,
         MinConfidence: float = ...,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
@@ -901,14 +966,15 @@
         """
         Starts asynchronous detection of inappropriate, unwanted, or offensive content
         in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_content_moderation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_content_moderation)
         """
+
     async def start_face_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         FaceAttributes: FaceAttributesType = ...,
@@ -916,14 +982,15 @@
     ) -> StartFaceDetectionResponseTypeDef:
         """
         Starts asynchronous detection of faces in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_face_detection)
         """
+
     async def start_face_search(
         self,
         *,
         Video: VideoTypeDef,
         CollectionId: str,
         ClientRequestToken: str = ...,
         FaceMatchThreshold: float = ...,
@@ -933,14 +1000,15 @@
         """
         Starts the asynchronous search for faces in a collection that match the faces of
         persons detected in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_face_search)
         """
+
     async def start_label_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
@@ -950,37 +1018,40 @@
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_label_detection)
         """
+
     async def start_person_tracking(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...
     ) -> StartPersonTrackingResponseTypeDef:
         """
         Starts the asynchronous tracking of a person's path in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_person_tracking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_person_tracking)
         """
+
     async def start_project_version(
         self, *, ProjectVersionArn: str, MinInferenceUnits: int, MaxInferenceUnits: int = ...
     ) -> StartProjectVersionResponseTypeDef:
         """
         Starts the running of the version of a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_project_version)
         """
+
     async def start_segment_detection(
         self,
         *,
         Video: VideoTypeDef,
         SegmentTypes: Sequence[SegmentTypeType],
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
@@ -989,27 +1060,29 @@
     ) -> StartSegmentDetectionResponseTypeDef:
         """
         Starts asynchronous detection of segment detection in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_segment_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_segment_detection)
         """
+
     async def start_stream_processor(
         self,
         *,
         Name: str,
         StartSelector: StreamProcessingStartSelectorTypeDef = ...,
         StopSelector: StreamProcessingStopSelectorTypeDef = ...
     ) -> StartStreamProcessorResponseTypeDef:
         """
         Starts processing a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_stream_processor)
         """
+
     async def start_text_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
@@ -1017,157 +1090,176 @@
     ) -> StartTextDetectionResponseTypeDef:
         """
         Starts asynchronous detection of text in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_text_detection)
         """
+
     async def stop_project_version(
         self, *, ProjectVersionArn: str
     ) -> StopProjectVersionResponseTypeDef:
         """
         Stops a running model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#stop_project_version)
         """
+
     async def stop_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops a running stream processor that was created by  CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#stop_stream_processor)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more key-value tags to an Amazon Rekognition collection, stream
         processor, or Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from an Amazon Rekognition collection, stream
         processor, or Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#untag_resource)
         """
+
     async def update_dataset_entries(
         self, *, DatasetArn: str, Changes: DatasetChangesTypeDef
     ) -> Dict[str, Any]:
         """
         Adds or updates one or more entries (images) in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_dataset_entries)
         """
+
     async def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_stream_processor)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_project_versions"]
     ) -> DescribeProjectVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_projects"]
     ) -> DescribeProjectsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_collections"]
     ) -> ListCollectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dataset_entries"]
     ) -> ListDatasetEntriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dataset_labels"]
     ) -> ListDatasetLabelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_faces"]) -> ListFacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_project_policies"]
     ) -> ListProjectPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_stream_processors"]
     ) -> ListStreamProcessorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_users"]) -> ListUsersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_paginator)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["project_version_running"]
     ) -> ProjectVersionRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["project_version_training_completed"]
     ) -> ProjectVersionTrainingCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "RekognitionClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
         """
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/literals.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/literals.pyi` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/paginator.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,167 +62,156 @@
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
     "ListUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeProjectVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectversionspaginator)
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeProjectVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectversionspaginator)
         """
 
-
 class DescribeProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectspaginator)
     """
 
     def paginate(
-        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectspaginator)
         """
 
-
 class ListCollectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listcollectionspaginator)
         """
 
-
 class ListDatasetEntriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetentriespaginator)
     """
 
     def paginate(
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetentriespaginator)
         """
 
-
 class ListDatasetLabelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetlabelspaginator)
     """
 
     def paginate(
-        self, *, DatasetArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DatasetArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetLabelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetlabelspaginator)
         """
 
-
 class ListFacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listfacespaginator)
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listfacespaginator)
         """
 
-
 class ListProjectPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listprojectpoliciespaginator)
     """
 
     def paginate(
-        self, *, ProjectArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listprojectpoliciespaginator)
         """
 
-
 class ListStreamProcessorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#liststreamprocessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamProcessorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#liststreamprocessorspaginator)
         """
 
-
 class ListUsersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/paginator.pyi` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,156 +62,167 @@
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
     "ListUsersPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeProjectVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectversionspaginator)
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeProjectVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectversionspaginator)
         """
 
+
 class DescribeProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectspaginator)
     """
 
     def paginate(
-        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectspaginator)
         """
 
+
 class ListCollectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listcollectionspaginator)
         """
 
+
 class ListDatasetEntriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetentriespaginator)
     """
 
     def paginate(
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetentriespaginator)
         """
 
+
 class ListDatasetLabelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetlabelspaginator)
     """
 
     def paginate(
-        self, *, DatasetArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DatasetArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetLabelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetlabelspaginator)
         """
 
+
 class ListFacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listfacespaginator)
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listfacespaginator)
         """
 
+
 class ListProjectPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listprojectpoliciespaginator)
     """
 
     def paginate(
-        self, *, ProjectArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listprojectpoliciespaginator)
         """
 
+
 class ListStreamProcessorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#liststreamprocessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamProcessorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#liststreamprocessorspaginator)
         """
 
+
 class ListUsersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/type_defs.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_rekognition.type_defs import AgeRangeTypeDef
 
-    data: AgeRangeTypeDef = {...}
+    data: AgeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -68,67 +68,57 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
+    "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
     "BoundingBoxTypeDef",
     "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
+    "BlobTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
+    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
-    "CopyProjectVersionResponseTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
-    "CreateCollectionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
     "LivenessOutputConfigTypeDef",
-    "CreateFaceLivenessSessionResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateProjectVersionResponseTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
-    "CreateStreamProcessorResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
-    "DeleteCollectionResponseTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
     "UnsuccessfulFaceDeletionTypeDef",
     "DeleteProjectPolicyRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteProjectVersionRequestRequestTypeDef",
-    "DeleteProjectVersionResponseTypeDef",
     "DeleteStreamProcessorRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeCollectionRequestRequestTypeDef",
-    "DescribeCollectionResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
-    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
@@ -166,100 +156,113 @@
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
     "ListCollectionsRequestRequestTypeDef",
-    "ListCollectionsResponseTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     "ListDatasetLabelsRequestRequestTypeDef",
-    "ListFacesRequestListFacesPaginateTypeDef",
     "ListFacesRequestRequestTypeDef",
-    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     "ListProjectPoliciesRequestRequestTypeDef",
     "ProjectPolicyTypeDef",
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
-    "PaginatorConfigTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
-    "PutProjectPolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchedFaceTypeDef",
     "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
     "TechnicalCueSegmentTypeDef",
+    "StartProjectVersionRequestRequestTypeDef",
+    "StartShotDetectionFilterTypeDef",
+    "StreamProcessingStopSelectorTypeDef",
+    "StopProjectVersionRequestRequestTypeDef",
+    "StopStreamProcessorRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "CopyProjectVersionResponseTypeDef",
+    "CreateCollectionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateFaceLivenessSessionResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateProjectVersionResponseTypeDef",
+    "CreateStreamProcessorResponseTypeDef",
+    "DeleteCollectionResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteProjectVersionResponseTypeDef",
+    "DescribeCollectionResponseTypeDef",
+    "ListCollectionsResponseTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutProjectPolicyResponseTypeDef",
     "StartCelebrityRecognitionResponseTypeDef",
     "StartContentModerationResponseTypeDef",
     "StartFaceDetectionResponseTypeDef",
     "StartFaceSearchResponseTypeDef",
     "StartLabelDetectionResponseTypeDef",
     "StartPersonTrackingResponseTypeDef",
-    "StartProjectVersionRequestRequestTypeDef",
     "StartProjectVersionResponseTypeDef",
-    "StartShotDetectionFilterTypeDef",
     "StartSegmentDetectionResponseTypeDef",
-    "StreamProcessingStopSelectorTypeDef",
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
-    "StopProjectVersionRequestRequestTypeDef",
     "StopProjectVersionResponseTypeDef",
-    "StopStreamProcessorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
     "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
     "SummaryTypeDef",
     "VideoTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
+    "DatasetChangesTypeDef",
+    "ImageTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
     "CreateFaceLivenessSessionRequestSettingsTypeDef",
-    "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
     "DeleteFacesResponseTypeDef",
+    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    "ListFacesRequestListFacesPaginateTypeDef",
+    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
+    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
+    "RegionOfInterestOutputTypeDef",
     "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -267,29 +270,30 @@
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
     "AssetTypeDef",
     "DatasetSourceTypeDef",
+    "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
+    "StartSegmentDetectionFiltersTypeDef",
+    "UpdateDatasetEntriesRequestRequestTypeDef",
     "CompareFacesRequestRequestTypeDef",
     "DetectCustomLabelsRequestRequestTypeDef",
     "DetectFacesRequestRequestTypeDef",
     "DetectProtectiveEquipmentRequestRequestTypeDef",
     "IndexFacesRequestRequestTypeDef",
     "RecognizeCelebritiesRequestRequestTypeDef",
     "SearchFacesByImageRequestRequestTypeDef",
     "SearchUsersByImageRequestRequestTypeDef",
-    "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
-    "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
@@ -302,28 +306,30 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
+    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
+    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
+    "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
+    "TrainingDataOutputTypeDef",
     "TrainingDataTypeDef",
     "ValidationDataTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
@@ -335,16 +341,20 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
+    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
+    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -390,14 +400,25 @@
     "AssociatedFaceTypeDef",
     {
         "FaceId": str,
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
 UnsuccessfulFaceAssociationTypeDef = TypedDict(
     "UnsuccessfulFaceAssociationTypeDef",
     {
         "FaceId": str,
         "UserId": str,
         "Confidence": float,
         "Reasons": List[UnsuccessfulFaceAssociationReasonType],
@@ -451,14 +472,15 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -515,14 +537,35 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
+_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_RequiredConnectedHomeSettingsOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+)
+_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_OptionalConnectedHomeSettingsOutputTypeDef",
+    {
+        "MinConfidence": float,
+    },
+    total=False,
+)
+
+
+class ConnectedHomeSettingsOutputTypeDef(
+    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
@@ -555,22 +598,14 @@
     {
         "S3Bucket": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-CopyProjectVersionResponseTypeDef = TypedDict(
-    "CopyProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CoversBodyPartTypeDef = TypedDict(
     "CoversBodyPartTypeDef",
     {
         "Confidence": float,
         "Value": bool,
     },
     total=False,
@@ -593,32 +628,14 @@
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
 
-CreateCollectionResponseTypeDef = TypedDict(
-    "CreateCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "CollectionArn": str,
-        "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLivenessOutputConfigTypeDef = TypedDict(
     "_RequiredLivenessOutputConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalLivenessOutputConfigTypeDef = TypedDict(
@@ -632,67 +649,35 @@
 
 class LivenessOutputConfigTypeDef(
     _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
 ):
     pass
 
 
-CreateFaceLivenessSessionResponseTypeDef = TypedDict(
-    "CreateFaceLivenessSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProjectVersionResponseTypeDef = TypedDict(
-    "CreateProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StreamProcessorDataSharingPreferenceTypeDef = TypedDict(
     "StreamProcessorDataSharingPreferenceTypeDef",
     {
         "OptIn": bool,
     },
 )
 
 StreamProcessorNotificationChannelTypeDef = TypedDict(
     "StreamProcessorNotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
     },
 )
 
-CreateStreamProcessorResponseTypeDef = TypedDict(
-    "CreateStreamProcessorResponseTypeDef",
-    {
-        "StreamProcessorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "CollectionId": str,
         "UserId": str,
     },
 )
@@ -707,21 +692,14 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
-DatasetChangesTypeDef = TypedDict(
-    "DatasetChangesTypeDef",
-    {
-        "GroundTruth": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 DatasetStatsTypeDef = TypedDict(
     "DatasetStatsTypeDef",
     {
         "LabeledEntries": int,
         "TotalEntries": int,
         "TotalLabels": int,
         "ErrorEntries": int,
@@ -754,22 +732,14 @@
 DeleteCollectionRequestRequestTypeDef = TypedDict(
     "DeleteCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DeleteCollectionResponseTypeDef = TypedDict(
-    "DeleteCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -817,37 +787,21 @@
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "Status": ProjectStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectVersionRequestRequestTypeDef = TypedDict(
     "DeleteProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
     },
 )
 
-DeleteProjectVersionResponseTypeDef = TypedDict(
-    "DeleteProjectVersionResponseTypeDef",
-    {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteStreamProcessorRequestRequestTypeDef = TypedDict(
     "DeleteStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -876,56 +830,31 @@
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DescribeCollectionResponseTypeDef = TypedDict(
-    "DescribeCollectionResponseTypeDef",
-    {
-        "FaceCount": int,
-        "FaceModelVersion": str,
-        "CollectionARN": str,
-        "CreationTimestamp": datetime,
-        "UserCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
-_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "VersionNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
-    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-):
-    pass
-
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -951,23 +880,14 @@
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    {
-        "ProjectNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -1495,67 +1415,23 @@
     "ParentTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCollectionsResponseTypeDef = TypedDict(
-    "ListCollectionsResponseTypeDef",
-    {
-        "CollectionIds": List[str],
-        "NextToken": str,
-        "FaceModelVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ContainsLabels": Sequence[str],
-        "Labeled": bool,
-        "SourceRefContains": str,
-        "HasErrors": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
@@ -1575,45 +1451,14 @@
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
-    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1628,38 +1473,14 @@
 
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_RequiredListFacesRequestListFacesPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_OptionalListFacesRequestListFacesPaginateTypeDef",
-    {
-        "UserId": str,
-        "FaceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFacesRequestListFacesPaginateTypeDef(
-    _RequiredListFacesRequestListFacesPaginateTypeDef,
-    _OptionalListFacesRequestListFacesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
@@ -1676,36 +1497,14 @@
 
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
-    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1734,22 +1533,14 @@
         "PolicyDocument": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamProcessorsRequestRequestTypeDef = TypedDict(
     "ListStreamProcessorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1767,44 +1558,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
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
         "CollectionId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1845,24 +1606,14 @@
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
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
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyDocument": str,
     },
@@ -1878,33 +1629,14 @@
 
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutProjectPolicyResponseTypeDef = TypedDict(
-    "PutProjectPolicyResponseTypeDef",
-    {
-        "PolicyRevisionId": str,
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
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1987,178 +1719,307 @@
     {
         "Type": TechnicalCueTypeType,
         "Confidence": float,
     },
     total=False,
 )
 
-StartCelebrityRecognitionResponseTypeDef = TypedDict(
-    "StartCelebrityRecognitionResponseTypeDef",
+_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
+        "MinInferenceUnits": int,
+    },
+)
+_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartProjectVersionRequestRequestTypeDef",
+    {
+        "MaxInferenceUnits": int,
     },
+    total=False,
 )
 
-StartContentModerationResponseTypeDef = TypedDict(
-    "StartContentModerationResponseTypeDef",
+
+class StartProjectVersionRequestRequestTypeDef(
+    _RequiredStartProjectVersionRequestRequestTypeDef,
+    _OptionalStartProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+
+StartShotDetectionFilterTypeDef = TypedDict(
+    "StartShotDetectionFilterTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MinSegmentConfidence": float,
     },
+    total=False,
 )
 
-StartFaceDetectionResponseTypeDef = TypedDict(
-    "StartFaceDetectionResponseTypeDef",
+StreamProcessingStopSelectorTypeDef = TypedDict(
+    "StreamProcessingStopSelectorTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxDurationInSeconds": int,
     },
+    total=False,
 )
 
-StartFaceSearchResponseTypeDef = TypedDict(
-    "StartFaceSearchResponseTypeDef",
+StopProjectVersionRequestRequestTypeDef = TypedDict(
+    "StopProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
     },
 )
 
-StartLabelDetectionResponseTypeDef = TypedDict(
-    "StartLabelDetectionResponseTypeDef",
+StopStreamProcessorRequestRequestTypeDef = TypedDict(
+    "StopStreamProcessorRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
 
-StartPersonTrackingResponseTypeDef = TypedDict(
-    "StartPersonTrackingResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartProjectVersionRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+CopyProjectVersionResponseTypeDef = TypedDict(
+    "CopyProjectVersionResponseTypeDef",
     {
         "ProjectVersionArn": str,
-        "MinInferenceUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartProjectVersionRequestRequestTypeDef",
+
+CreateCollectionResponseTypeDef = TypedDict(
+    "CreateCollectionResponseTypeDef",
     {
-        "MaxInferenceUnits": int,
+        "StatusCode": int,
+        "CollectionArn": str,
+        "FaceModelVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class StartProjectVersionRequestRequestTypeDef(
-    _RequiredStartProjectVersionRequestRequestTypeDef,
-    _OptionalStartProjectVersionRequestRequestTypeDef,
-):
-    pass
+CreateFaceLivenessSessionResponseTypeDef = TypedDict(
+    "CreateFaceLivenessSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-StartProjectVersionResponseTypeDef = TypedDict(
-    "StartProjectVersionResponseTypeDef",
+CreateProjectVersionResponseTypeDef = TypedDict(
+    "CreateProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamProcessorResponseTypeDef = TypedDict(
+    "CreateStreamProcessorResponseTypeDef",
+    {
+        "StreamProcessorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCollectionResponseTypeDef = TypedDict(
+    "DeleteCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Status": ProjectStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectVersionResponseTypeDef = TypedDict(
+    "DeleteProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartShotDetectionFilterTypeDef = TypedDict(
-    "StartShotDetectionFilterTypeDef",
+DescribeCollectionResponseTypeDef = TypedDict(
+    "DescribeCollectionResponseTypeDef",
     {
-        "MinSegmentConfidence": float,
+        "FaceCount": int,
+        "FaceModelVersion": str,
+        "CollectionARN": str,
+        "CreationTimestamp": datetime,
+        "UserCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartSegmentDetectionResponseTypeDef = TypedDict(
-    "StartSegmentDetectionResponseTypeDef",
+ListCollectionsResponseTypeDef = TypedDict(
+    "ListCollectionsResponseTypeDef",
+    {
+        "CollectionIds": List[str],
+        "NextToken": str,
+        "FaceModelVersions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProjectPolicyResponseTypeDef = TypedDict(
+    "PutProjectPolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCelebrityRecognitionResponseTypeDef = TypedDict(
+    "StartCelebrityRecognitionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamProcessingStopSelectorTypeDef = TypedDict(
-    "StreamProcessingStopSelectorTypeDef",
+StartContentModerationResponseTypeDef = TypedDict(
+    "StartContentModerationResponseTypeDef",
     {
-        "MaxDurationInSeconds": int,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartStreamProcessorResponseTypeDef = TypedDict(
-    "StartStreamProcessorResponseTypeDef",
+StartFaceDetectionResponseTypeDef = TypedDict(
+    "StartFaceDetectionResponseTypeDef",
     {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTextDetectionResponseTypeDef = TypedDict(
-    "StartTextDetectionResponseTypeDef",
+StartFaceSearchResponseTypeDef = TypedDict(
+    "StartFaceSearchResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionRequestRequestTypeDef = TypedDict(
-    "StopProjectVersionRequestRequestTypeDef",
+StartLabelDetectionResponseTypeDef = TypedDict(
+    "StartLabelDetectionResponseTypeDef",
     {
-        "ProjectVersionArn": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionResponseTypeDef = TypedDict(
-    "StopProjectVersionResponseTypeDef",
+StartPersonTrackingResponseTypeDef = TypedDict(
+    "StartPersonTrackingResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartProjectVersionResponseTypeDef = TypedDict(
+    "StartProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopStreamProcessorRequestRequestTypeDef = TypedDict(
-    "StopStreamProcessorRequestRequestTypeDef",
+StartSegmentDetectionResponseTypeDef = TypedDict(
+    "StartSegmentDetectionResponseTypeDef",
     {
-        "Name": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartStreamProcessorResponseTypeDef = TypedDict(
+    "StartStreamProcessorResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartTextDetectionResponseTypeDef = TypedDict(
+    "StartTextDetectionResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopProjectVersionResponseTypeDef = TypedDict(
+    "StopProjectVersionResponseTypeDef",
+    {
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateFacesResponseTypeDef = TypedDict(
     "AssociateFacesResponseTypeDef",
     {
         "AssociatedFaces": List[AssociatedFaceTypeDef],
         "UnsuccessfulFaceAssociations": List[UnsuccessfulFaceAssociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedSourceImageFaceTypeDef = TypedDict(
     "ComparedSourceImageFaceTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
@@ -2195,23 +2056,14 @@
     "GroundTruthManifestTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
@@ -2229,21 +2081,37 @@
     {
         "MinSegmentConfidence": float,
         "BlackFrame": BlackFrameTypeDef,
     },
     total=False,
 )
 
+DatasetChangesTypeDef = TypedDict(
+    "DatasetChangesTypeDef",
+    {
+        "GroundTruth": BlobTypeDef,
+    },
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "Bytes": BlobTypeDef,
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 GetCelebrityInfoResponseTypeDef = TypedDict(
     "GetCelebrityInfoResponseTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "KnownGender": KnownGenderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
@@ -2320,22 +2188,14 @@
     {
         "OutputConfig": LivenessOutputConfigTypeDef,
         "AuditImagesLimit": int,
     },
     total=False,
 )
 
-UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "UpdateDatasetEntriesRequestRequestTypeDef",
-    {
-        "DatasetArn": str,
-        "Changes": DatasetChangesTypeDef,
-    },
-)
-
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
@@ -2366,18 +2226,182 @@
 )
 
 DeleteFacesResponseTypeDef = TypedDict(
     "DeleteFacesResponseTypeDef",
     {
         "DeletedFaces": List[str],
         "UnsuccessfulFaceDeletions": List[UnsuccessfulFaceDeletionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "VersionNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
+    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+):
+    pass
+
+
+DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    {
+        "ProjectNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ContainsLabels": Sequence[str],
+        "Labeled": bool,
+        "SourceRefContains": str,
+        "HasErrors": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
+    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_RequiredListFacesRequestListFacesPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_OptionalListFacesRequestListFacesPaginateTypeDef",
+    {
+        "UserId": str,
+        "FaceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFacesRequestListFacesPaginateTypeDef(
+    _RequiredListFacesRequestListFacesPaginateTypeDef,
+    _OptionalListFacesRequestListFacesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
+    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+):
+    pass
+
+
+ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
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
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
@@ -2471,25 +2495,25 @@
 
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFacesResponseTypeDef = TypedDict(
     "DisassociateFacesResponseTypeDef",
     {
         "DisassociatedFaces": List[DisassociatedFaceTypeDef],
         "UnsuccessfulFaceDisassociations": List[UnsuccessfulFaceDisassociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DistributeDatasetEntriesRequestRequestTypeDef = TypedDict(
     "DistributeDatasetEntriesRequestRequestTypeDef",
     {
         "Datasets": Sequence[DistributeDatasetTypeDef],
@@ -2516,14 +2540,23 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
+StreamProcessorSettingsOutputTypeDef = TypedDict(
+    "StreamProcessorSettingsOutputTypeDef",
+    {
+        "FaceSearch": FaceSearchSettingsTypeDef,
+        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
@@ -2534,14 +2567,23 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
+RegionOfInterestOutputTypeDef = TypedDict(
+    "RegionOfInterestOutputTypeDef",
+    {
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": List[PointTypeDef],
+    },
+    total=False,
+)
+
 RegionOfInterestTypeDef = TypedDict(
     "RegionOfInterestTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
@@ -2584,33 +2626,33 @@
 )
 
 ListProjectPoliciesResponseTypeDef = TypedDict(
     "ListProjectPoliciesResponseTypeDef",
     {
         "ProjectPolicies": List[ProjectPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamProcessorsResponseTypeDef = TypedDict(
     "ListStreamProcessorsResponseTypeDef",
     {
         "NextToken": str,
         "StreamProcessors": List[StreamProcessorTypeDef],
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
 
 UserMatchTypeDef = TypedDict(
     "UserMatchTypeDef",
     {
         "Similarity": float,
@@ -2658,27 +2700,27 @@
 
 ListFacesResponseTypeDef = TypedDict(
     "ListFacesResponseTypeDef",
     {
         "Faces": List[FaceTypeDef],
         "NextToken": str,
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceLivenessSessionResultsResponseTypeDef = TypedDict(
     "GetFaceLivenessSessionResultsResponseTypeDef",
     {
         "SessionId": str,
         "Status": LivenessSessionStatusType,
         "Confidence": float,
         "ReferenceImage": AuditImageTypeDef,
         "AuditImages": List[AuditImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
@@ -2691,14 +2733,163 @@
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
         "DatasetArn": str,
     },
     total=False,
 )
 
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartCelebrityRecognitionRequestRequestTypeDef(
+    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
+    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartContentModerationRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartContentModerationRequestRequestTypeDef",
+    {
+        "MinConfidence": float,
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartContentModerationRequestRequestTypeDef(
+    _RequiredStartContentModerationRequestRequestTypeDef,
+    _OptionalStartContentModerationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceDetectionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceDetectionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "FaceAttributes": FaceAttributesType,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartFaceDetectionRequestRequestTypeDef(
+    _RequiredStartFaceDetectionRequestRequestTypeDef,
+    _OptionalStartFaceDetectionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceSearchRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+        "CollectionId": str,
+    },
+)
+_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceSearchRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "FaceMatchThreshold": float,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartFaceSearchRequestRequestTypeDef(
+    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
+
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetEntriesRequestRequestTypeDef",
+    {
+        "DatasetArn": str,
+        "Changes": DatasetChangesTypeDef,
+    },
+)
+
 _RequiredCompareFacesRequestRequestTypeDef = TypedDict(
     "_RequiredCompareFacesRequestRequestTypeDef",
     {
         "SourceImage": ImageTypeDef,
         "TargetImage": ImageTypeDef,
     },
 )
@@ -2863,155 +3054,14 @@
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
-_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartCelebrityRecognitionRequestRequestTypeDef(
-    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
-    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartContentModerationRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartContentModerationRequestRequestTypeDef",
-    {
-        "MinConfidence": float,
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartContentModerationRequestRequestTypeDef(
-    _RequiredStartContentModerationRequestRequestTypeDef,
-    _OptionalStartContentModerationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceDetectionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceDetectionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "FaceAttributes": FaceAttributesType,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartFaceDetectionRequestRequestTypeDef(
-    _RequiredStartFaceDetectionRequestRequestTypeDef,
-    _OptionalStartFaceDetectionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceSearchRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-        "CollectionId": str,
-    },
-)
-_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceSearchRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "FaceMatchThreshold": float,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartFaceSearchRequestRequestTypeDef(
-    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
-
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
 CelebrityTypeDef = TypedDict(
     "CelebrityTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Face": ComparedFaceTypeDef,
@@ -3039,15 +3089,15 @@
         "ModerationLabels": List[ContentModerationDetectionTypeDef],
         "NextToken": str,
         "ModerationModelVersion": str,
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectiveEquipmentBodyPartTypeDef = TypedDict(
     "ProtectiveEquipmentBodyPartTypeDef",
     {
         "Name": BodyPartType,
@@ -3067,33 +3117,33 @@
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetLabelsResponseTypeDef = TypedDict(
     "ListDatasetLabelsResponseTypeDef",
     {
         "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProjectsResponseTypeDef = TypedDict(
     "DescribeProjectsResponseTypeDef",
     {
         "ProjectDescriptions": List[ProjectDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectLabelsImagePropertiesTypeDef = TypedDict(
     "DetectLabelsImagePropertiesTypeDef",
     {
         "Quality": DetectLabelsImageQualityTypeDef,
@@ -3183,15 +3233,15 @@
 )
 
 DetectFacesResponseTypeDef = TypedDict(
     "DetectFacesResponseTypeDef",
     {
         "FaceDetails": List[FaceDetailTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FaceDetectionTypeDef = TypedDict(
     "FaceDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3241,14 +3291,17 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
+StreamProcessorSettingsUnionTypeDef = Union[
+    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
+]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3273,48 +3326,24 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3360,66 +3389,36 @@
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsTypeDef,
+        "Settings": StreamProcessorSettingsOutputTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestTypeDef],
+        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
@@ -3428,48 +3427,65 @@
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesByImageResponseTypeDef = TypedDict(
     "SearchFacesByImageResponseTypeDef",
     {
         "SearchedFaceBoundingBox": BoundingBoxTypeDef,
         "SearchedFaceConfidence": float,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesResponseTypeDef = TypedDict(
     "SearchFacesResponseTypeDef",
     {
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestingDataOutputTypeDef = TypedDict(
+    "TestingDataOutputTypeDef",
+    {
+        "Assets": List[AssetTypeDef],
+        "AutoCreate": bool,
     },
+    total=False,
 )
 
 TestingDataTypeDef = TypedDict(
     "TestingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
+TrainingDataOutputTypeDef = TypedDict(
+    "TrainingDataOutputTypeDef",
+    {
+        "Assets": List[AssetTypeDef],
+    },
+    total=False,
+)
+
 TrainingDataTypeDef = TypedDict(
     "TrainingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
@@ -3532,27 +3548,27 @@
 
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompareFacesResponseTypeDef = TypedDict(
     "CompareFacesResponseTypeDef",
     {
         "SourceImageFace": ComparedSourceImageFaceTypeDef,
         "FaceMatches": List[CompareFacesMatchTypeDef],
         "UnmatchedFaces": List[ComparedFaceTypeDef],
         "SourceImageOrientationCorrection": OrientationCorrectionType,
         "TargetImageOrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
@@ -3566,15 +3582,15 @@
 DetectLabelsResponseTypeDef = TypedDict(
     "DetectLabelsResponseTypeDef",
     {
         "Labels": List[LabelTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "LabelModelVersion": str,
         "ImageProperties": DetectLabelsImagePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3602,15 +3618,15 @@
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3632,43 +3648,43 @@
 IndexFacesResponseTypeDef = TypedDict(
     "IndexFacesResponseTypeDef",
     {
         "FaceRecords": List[FaceRecordTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "FaceModelVersion": str,
         "UnindexedFaces": List[UnindexedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchUsersByImageResponseTypeDef = TypedDict(
     "SearchUsersByImageResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceDetailsTypeDef,
         "UnsearchedFaces": List[UnsearchedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectCustomLabelsResponseTypeDef = TypedDict(
     "DetectCustomLabelsResponseTypeDef",
     {
         "CustomLabels": List[CustomLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectTextResponseTypeDef = TypedDict(
     "DetectTextResponseTypeDef",
     {
         "TextDetections": List[TextDetectionTypeDef],
         "TextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TextDetectionResultTypeDef = TypedDict(
     "TextDetectionResultTypeDef",
     {
         "Timestamp": int,
@@ -3694,14 +3710,69 @@
 
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3719,14 +3790,15 @@
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
 
+TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3746,41 +3818,42 @@
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
 
+TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataTypeDef,
-        "Output": TestingDataTypeDef,
+        "Input": TestingDataOutputTypeDef,
+        "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataTypeDef,
-        "Output": TrainingDataTypeDef,
+        "Input": TrainingDataOutputTypeDef,
+        "Output": TrainingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
     {
         "ProtectiveEquipmentModelVersion": str,
         "Persons": List[ProtectiveEquipmentPersonTypeDef],
         "Summary": ProtectiveEquipmentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLabelDetectionResponseTypeDef = TypedDict(
     "GetLabelDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
@@ -3789,60 +3862,60 @@
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
     "GetCelebrityRecognitionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
@@ -3850,15 +3923,15 @@
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
@@ -3881,10 +3954,10 @@
 )
 
 DescribeProjectVersionsResponseTypeDef = TypedDict(
     "DescribeProjectVersionsResponseTypeDef",
     {
         "ProjectVersionDescriptions": List[ProjectVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/type_defs.pyi` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_rekognition.type_defs import AgeRangeTypeDef
 
-    data: AgeRangeTypeDef = {...}
+    data: AgeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -67,67 +67,57 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
+    "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
     "BoundingBoxTypeDef",
     "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
+    "BlobTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
+    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
-    "CopyProjectVersionResponseTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
-    "CreateCollectionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
     "LivenessOutputConfigTypeDef",
-    "CreateFaceLivenessSessionResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateProjectVersionResponseTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
-    "CreateStreamProcessorResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
-    "DeleteCollectionResponseTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
     "UnsuccessfulFaceDeletionTypeDef",
     "DeleteProjectPolicyRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteProjectVersionRequestRequestTypeDef",
-    "DeleteProjectVersionResponseTypeDef",
     "DeleteStreamProcessorRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeCollectionRequestRequestTypeDef",
-    "DescribeCollectionResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
-    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
@@ -165,100 +155,113 @@
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
     "ListCollectionsRequestRequestTypeDef",
-    "ListCollectionsResponseTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     "ListDatasetLabelsRequestRequestTypeDef",
-    "ListFacesRequestListFacesPaginateTypeDef",
     "ListFacesRequestRequestTypeDef",
-    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     "ListProjectPoliciesRequestRequestTypeDef",
     "ProjectPolicyTypeDef",
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
-    "PaginatorConfigTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
-    "PutProjectPolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchedFaceTypeDef",
     "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
     "TechnicalCueSegmentTypeDef",
+    "StartProjectVersionRequestRequestTypeDef",
+    "StartShotDetectionFilterTypeDef",
+    "StreamProcessingStopSelectorTypeDef",
+    "StopProjectVersionRequestRequestTypeDef",
+    "StopStreamProcessorRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "CopyProjectVersionResponseTypeDef",
+    "CreateCollectionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateFaceLivenessSessionResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateProjectVersionResponseTypeDef",
+    "CreateStreamProcessorResponseTypeDef",
+    "DeleteCollectionResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteProjectVersionResponseTypeDef",
+    "DescribeCollectionResponseTypeDef",
+    "ListCollectionsResponseTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutProjectPolicyResponseTypeDef",
     "StartCelebrityRecognitionResponseTypeDef",
     "StartContentModerationResponseTypeDef",
     "StartFaceDetectionResponseTypeDef",
     "StartFaceSearchResponseTypeDef",
     "StartLabelDetectionResponseTypeDef",
     "StartPersonTrackingResponseTypeDef",
-    "StartProjectVersionRequestRequestTypeDef",
     "StartProjectVersionResponseTypeDef",
-    "StartShotDetectionFilterTypeDef",
     "StartSegmentDetectionResponseTypeDef",
-    "StreamProcessingStopSelectorTypeDef",
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
-    "StopProjectVersionRequestRequestTypeDef",
     "StopProjectVersionResponseTypeDef",
-    "StopStreamProcessorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
     "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
     "SummaryTypeDef",
     "VideoTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
+    "DatasetChangesTypeDef",
+    "ImageTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
     "CreateFaceLivenessSessionRequestSettingsTypeDef",
-    "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
     "DeleteFacesResponseTypeDef",
+    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    "ListFacesRequestListFacesPaginateTypeDef",
+    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
+    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
+    "RegionOfInterestOutputTypeDef",
     "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -266,29 +269,30 @@
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
     "AssetTypeDef",
     "DatasetSourceTypeDef",
+    "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
+    "StartSegmentDetectionFiltersTypeDef",
+    "UpdateDatasetEntriesRequestRequestTypeDef",
     "CompareFacesRequestRequestTypeDef",
     "DetectCustomLabelsRequestRequestTypeDef",
     "DetectFacesRequestRequestTypeDef",
     "DetectProtectiveEquipmentRequestRequestTypeDef",
     "IndexFacesRequestRequestTypeDef",
     "RecognizeCelebritiesRequestRequestTypeDef",
     "SearchFacesByImageRequestRequestTypeDef",
     "SearchUsersByImageRequestRequestTypeDef",
-    "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
-    "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
@@ -301,28 +305,30 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
+    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
+    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
+    "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
+    "TrainingDataOutputTypeDef",
     "TrainingDataTypeDef",
     "ValidationDataTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
@@ -334,16 +340,20 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
+    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
+    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -387,14 +397,25 @@
     "AssociatedFaceTypeDef",
     {
         "FaceId": str,
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
 UnsuccessfulFaceAssociationTypeDef = TypedDict(
     "UnsuccessfulFaceAssociationTypeDef",
     {
         "FaceId": str,
         "UserId": str,
         "Confidence": float,
         "Reasons": List[UnsuccessfulFaceAssociationReasonType],
@@ -448,14 +469,15 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -512,14 +534,33 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
+_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_RequiredConnectedHomeSettingsOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+)
+_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_OptionalConnectedHomeSettingsOutputTypeDef",
+    {
+        "MinConfidence": float,
+    },
+    total=False,
+)
+
+class ConnectedHomeSettingsOutputTypeDef(
+    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
+):
+    pass
+
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
@@ -550,22 +591,14 @@
     {
         "S3Bucket": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-CopyProjectVersionResponseTypeDef = TypedDict(
-    "CopyProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CoversBodyPartTypeDef = TypedDict(
     "CoversBodyPartTypeDef",
     {
         "Confidence": float,
         "Value": bool,
     },
     total=False,
@@ -586,32 +619,14 @@
 )
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
-CreateCollectionResponseTypeDef = TypedDict(
-    "CreateCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "CollectionArn": str,
-        "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLivenessOutputConfigTypeDef = TypedDict(
     "_RequiredLivenessOutputConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalLivenessOutputConfigTypeDef = TypedDict(
@@ -623,67 +638,35 @@
 )
 
 class LivenessOutputConfigTypeDef(
     _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
 ):
     pass
 
-CreateFaceLivenessSessionResponseTypeDef = TypedDict(
-    "CreateFaceLivenessSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProjectVersionResponseTypeDef = TypedDict(
-    "CreateProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StreamProcessorDataSharingPreferenceTypeDef = TypedDict(
     "StreamProcessorDataSharingPreferenceTypeDef",
     {
         "OptIn": bool,
     },
 )
 
 StreamProcessorNotificationChannelTypeDef = TypedDict(
     "StreamProcessorNotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
     },
 )
 
-CreateStreamProcessorResponseTypeDef = TypedDict(
-    "CreateStreamProcessorResponseTypeDef",
-    {
-        "StreamProcessorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "CollectionId": str,
         "UserId": str,
     },
 )
@@ -696,21 +679,14 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-DatasetChangesTypeDef = TypedDict(
-    "DatasetChangesTypeDef",
-    {
-        "GroundTruth": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 DatasetStatsTypeDef = TypedDict(
     "DatasetStatsTypeDef",
     {
         "LabeledEntries": int,
         "TotalEntries": int,
         "TotalLabels": int,
         "ErrorEntries": int,
@@ -743,22 +719,14 @@
 DeleteCollectionRequestRequestTypeDef = TypedDict(
     "DeleteCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DeleteCollectionResponseTypeDef = TypedDict(
-    "DeleteCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -804,37 +772,21 @@
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "Status": ProjectStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectVersionRequestRequestTypeDef = TypedDict(
     "DeleteProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
     },
 )
 
-DeleteProjectVersionResponseTypeDef = TypedDict(
-    "DeleteProjectVersionResponseTypeDef",
-    {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteStreamProcessorRequestRequestTypeDef = TypedDict(
     "DeleteStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -861,54 +813,31 @@
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DescribeCollectionResponseTypeDef = TypedDict(
-    "DescribeCollectionResponseTypeDef",
-    {
-        "FaceCount": int,
-        "FaceModelVersion": str,
-        "CollectionARN": str,
-        "CreationTimestamp": datetime,
-        "UserCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
-_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "VersionNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
-    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-):
-    pass
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -932,23 +861,14 @@
 
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
-DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    {
-        "ProjectNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -1458,65 +1378,23 @@
     "ParentTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCollectionsResponseTypeDef = TypedDict(
-    "ListCollectionsResponseTypeDef",
-    {
-        "CollectionIds": List[str],
-        "NextToken": str,
-        "FaceModelVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ContainsLabels": Sequence[str],
-        "Labeled": bool,
-        "SourceRefContains": str,
-        "HasErrors": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
@@ -1534,43 +1412,14 @@
 
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
-    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1583,36 +1432,14 @@
 )
 
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_RequiredListFacesRequestListFacesPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_OptionalListFacesRequestListFacesPaginateTypeDef",
-    {
-        "UserId": str,
-        "FaceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFacesRequestListFacesPaginateTypeDef(
-    _RequiredListFacesRequestListFacesPaginateTypeDef,
-    _OptionalListFacesRequestListFacesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
@@ -1627,34 +1454,14 @@
 )
 
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
-    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1681,22 +1488,14 @@
         "PolicyDocument": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamProcessorsRequestRequestTypeDef = TypedDict(
     "ListStreamProcessorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1714,42 +1513,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
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
         "CollectionId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1788,24 +1559,14 @@
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
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
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyDocument": str,
     },
@@ -1819,33 +1580,14 @@
 )
 
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
-PutProjectPolicyResponseTypeDef = TypedDict(
-    "PutProjectPolicyResponseTypeDef",
-    {
-        "PolicyRevisionId": str,
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
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1924,176 +1666,305 @@
     {
         "Type": TechnicalCueTypeType,
         "Confidence": float,
     },
     total=False,
 )
 
-StartCelebrityRecognitionResponseTypeDef = TypedDict(
-    "StartCelebrityRecognitionResponseTypeDef",
+_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
+        "MinInferenceUnits": int,
     },
 )
+_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartProjectVersionRequestRequestTypeDef",
+    {
+        "MaxInferenceUnits": int,
+    },
+    total=False,
+)
 
-StartContentModerationResponseTypeDef = TypedDict(
-    "StartContentModerationResponseTypeDef",
+class StartProjectVersionRequestRequestTypeDef(
+    _RequiredStartProjectVersionRequestRequestTypeDef,
+    _OptionalStartProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+StartShotDetectionFilterTypeDef = TypedDict(
+    "StartShotDetectionFilterTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MinSegmentConfidence": float,
     },
+    total=False,
 )
 
-StartFaceDetectionResponseTypeDef = TypedDict(
-    "StartFaceDetectionResponseTypeDef",
+StreamProcessingStopSelectorTypeDef = TypedDict(
+    "StreamProcessingStopSelectorTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxDurationInSeconds": int,
     },
+    total=False,
 )
 
-StartFaceSearchResponseTypeDef = TypedDict(
-    "StartFaceSearchResponseTypeDef",
+StopProjectVersionRequestRequestTypeDef = TypedDict(
+    "StopProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
     },
 )
 
-StartLabelDetectionResponseTypeDef = TypedDict(
-    "StartLabelDetectionResponseTypeDef",
+StopStreamProcessorRequestRequestTypeDef = TypedDict(
+    "StopStreamProcessorRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
 
-StartPersonTrackingResponseTypeDef = TypedDict(
-    "StartPersonTrackingResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartProjectVersionRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+CopyProjectVersionResponseTypeDef = TypedDict(
+    "CopyProjectVersionResponseTypeDef",
     {
         "ProjectVersionArn": str,
-        "MinInferenceUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartProjectVersionRequestRequestTypeDef",
+
+CreateCollectionResponseTypeDef = TypedDict(
+    "CreateCollectionResponseTypeDef",
     {
-        "MaxInferenceUnits": int,
+        "StatusCode": int,
+        "CollectionArn": str,
+        "FaceModelVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartProjectVersionRequestRequestTypeDef(
-    _RequiredStartProjectVersionRequestRequestTypeDef,
-    _OptionalStartProjectVersionRequestRequestTypeDef,
-):
-    pass
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-StartProjectVersionResponseTypeDef = TypedDict(
-    "StartProjectVersionResponseTypeDef",
+CreateFaceLivenessSessionResponseTypeDef = TypedDict(
+    "CreateFaceLivenessSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectVersionResponseTypeDef = TypedDict(
+    "CreateProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamProcessorResponseTypeDef = TypedDict(
+    "CreateStreamProcessorResponseTypeDef",
+    {
+        "StreamProcessorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCollectionResponseTypeDef = TypedDict(
+    "DeleteCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Status": ProjectStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectVersionResponseTypeDef = TypedDict(
+    "DeleteProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartShotDetectionFilterTypeDef = TypedDict(
-    "StartShotDetectionFilterTypeDef",
+DescribeCollectionResponseTypeDef = TypedDict(
+    "DescribeCollectionResponseTypeDef",
     {
-        "MinSegmentConfidence": float,
+        "FaceCount": int,
+        "FaceModelVersion": str,
+        "CollectionARN": str,
+        "CreationTimestamp": datetime,
+        "UserCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartSegmentDetectionResponseTypeDef = TypedDict(
-    "StartSegmentDetectionResponseTypeDef",
+ListCollectionsResponseTypeDef = TypedDict(
+    "ListCollectionsResponseTypeDef",
+    {
+        "CollectionIds": List[str],
+        "NextToken": str,
+        "FaceModelVersions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProjectPolicyResponseTypeDef = TypedDict(
+    "PutProjectPolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCelebrityRecognitionResponseTypeDef = TypedDict(
+    "StartCelebrityRecognitionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamProcessingStopSelectorTypeDef = TypedDict(
-    "StreamProcessingStopSelectorTypeDef",
+StartContentModerationResponseTypeDef = TypedDict(
+    "StartContentModerationResponseTypeDef",
     {
-        "MaxDurationInSeconds": int,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartStreamProcessorResponseTypeDef = TypedDict(
-    "StartStreamProcessorResponseTypeDef",
+StartFaceDetectionResponseTypeDef = TypedDict(
+    "StartFaceDetectionResponseTypeDef",
     {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTextDetectionResponseTypeDef = TypedDict(
-    "StartTextDetectionResponseTypeDef",
+StartFaceSearchResponseTypeDef = TypedDict(
+    "StartFaceSearchResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionRequestRequestTypeDef = TypedDict(
-    "StopProjectVersionRequestRequestTypeDef",
+StartLabelDetectionResponseTypeDef = TypedDict(
+    "StartLabelDetectionResponseTypeDef",
     {
-        "ProjectVersionArn": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionResponseTypeDef = TypedDict(
-    "StopProjectVersionResponseTypeDef",
+StartPersonTrackingResponseTypeDef = TypedDict(
+    "StartPersonTrackingResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartProjectVersionResponseTypeDef = TypedDict(
+    "StartProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopStreamProcessorRequestRequestTypeDef = TypedDict(
-    "StopStreamProcessorRequestRequestTypeDef",
+StartSegmentDetectionResponseTypeDef = TypedDict(
+    "StartSegmentDetectionResponseTypeDef",
     {
-        "Name": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartStreamProcessorResponseTypeDef = TypedDict(
+    "StartStreamProcessorResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartTextDetectionResponseTypeDef = TypedDict(
+    "StartTextDetectionResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopProjectVersionResponseTypeDef = TypedDict(
+    "StopProjectVersionResponseTypeDef",
+    {
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateFacesResponseTypeDef = TypedDict(
     "AssociateFacesResponseTypeDef",
     {
         "AssociatedFaces": List[AssociatedFaceTypeDef],
         "UnsuccessfulFaceAssociations": List[UnsuccessfulFaceAssociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedSourceImageFaceTypeDef = TypedDict(
     "ComparedSourceImageFaceTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
@@ -2130,23 +2001,14 @@
     "GroundTruthManifestTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
@@ -2164,21 +2026,37 @@
     {
         "MinSegmentConfidence": float,
         "BlackFrame": BlackFrameTypeDef,
     },
     total=False,
 )
 
+DatasetChangesTypeDef = TypedDict(
+    "DatasetChangesTypeDef",
+    {
+        "GroundTruth": BlobTypeDef,
+    },
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "Bytes": BlobTypeDef,
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 GetCelebrityInfoResponseTypeDef = TypedDict(
     "GetCelebrityInfoResponseTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "KnownGender": KnownGenderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
@@ -2253,22 +2131,14 @@
     {
         "OutputConfig": LivenessOutputConfigTypeDef,
         "AuditImagesLimit": int,
     },
     total=False,
 )
 
-UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "UpdateDatasetEntriesRequestRequestTypeDef",
-    {
-        "DatasetArn": str,
-        "Changes": DatasetChangesTypeDef,
-    },
-)
-
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
@@ -2299,17 +2169,169 @@
 )
 
 DeleteFacesResponseTypeDef = TypedDict(
     "DeleteFacesResponseTypeDef",
     {
         "DeletedFaces": List[str],
         "UnsuccessfulFaceDeletions": List[UnsuccessfulFaceDeletionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "VersionNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
+    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+):
+    pass
+
+DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    {
+        "ProjectNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ContainsLabels": Sequence[str],
+        "Labeled": bool,
+        "SourceRefContains": str,
+        "HasErrors": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
+    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_RequiredListFacesRequestListFacesPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_OptionalListFacesRequestListFacesPaginateTypeDef",
+    {
+        "UserId": str,
+        "FaceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFacesRequestListFacesPaginateTypeDef(
+    _RequiredListFacesRequestListFacesPaginateTypeDef,
+    _OptionalListFacesRequestListFacesPaginateTypeDef,
+):
+    pass
+
+_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
+    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+):
+    pass
+
+ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "CollectionId": str,
     },
 )
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
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
 
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
@@ -2400,25 +2422,25 @@
 
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFacesResponseTypeDef = TypedDict(
     "DisassociateFacesResponseTypeDef",
     {
         "DisassociatedFaces": List[DisassociatedFaceTypeDef],
         "UnsuccessfulFaceDisassociations": List[UnsuccessfulFaceDisassociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DistributeDatasetEntriesRequestRequestTypeDef = TypedDict(
     "DistributeDatasetEntriesRequestRequestTypeDef",
     {
         "Datasets": Sequence[DistributeDatasetTypeDef],
@@ -2445,14 +2467,23 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
+StreamProcessorSettingsOutputTypeDef = TypedDict(
+    "StreamProcessorSettingsOutputTypeDef",
+    {
+        "FaceSearch": FaceSearchSettingsTypeDef,
+        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
@@ -2463,14 +2494,23 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
+RegionOfInterestOutputTypeDef = TypedDict(
+    "RegionOfInterestOutputTypeDef",
+    {
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": List[PointTypeDef],
+    },
+    total=False,
+)
+
 RegionOfInterestTypeDef = TypedDict(
     "RegionOfInterestTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
@@ -2511,33 +2551,33 @@
 )
 
 ListProjectPoliciesResponseTypeDef = TypedDict(
     "ListProjectPoliciesResponseTypeDef",
     {
         "ProjectPolicies": List[ProjectPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamProcessorsResponseTypeDef = TypedDict(
     "ListStreamProcessorsResponseTypeDef",
     {
         "NextToken": str,
         "StreamProcessors": List[StreamProcessorTypeDef],
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
 
 UserMatchTypeDef = TypedDict(
     "UserMatchTypeDef",
     {
         "Similarity": float,
@@ -2585,27 +2625,27 @@
 
 ListFacesResponseTypeDef = TypedDict(
     "ListFacesResponseTypeDef",
     {
         "Faces": List[FaceTypeDef],
         "NextToken": str,
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceLivenessSessionResultsResponseTypeDef = TypedDict(
     "GetFaceLivenessSessionResultsResponseTypeDef",
     {
         "SessionId": str,
         "Status": LivenessSessionStatusType,
         "Confidence": float,
         "ReferenceImage": AuditImageTypeDef,
         "AuditImages": List[AuditImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
@@ -2618,14 +2658,153 @@
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
         "DatasetArn": str,
     },
     total=False,
 )
 
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartCelebrityRecognitionRequestRequestTypeDef(
+    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
+    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartContentModerationRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartContentModerationRequestRequestTypeDef",
+    {
+        "MinConfidence": float,
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartContentModerationRequestRequestTypeDef(
+    _RequiredStartContentModerationRequestRequestTypeDef,
+    _OptionalStartContentModerationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceDetectionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceDetectionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "FaceAttributes": FaceAttributesType,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartFaceDetectionRequestRequestTypeDef(
+    _RequiredStartFaceDetectionRequestRequestTypeDef,
+    _OptionalStartFaceDetectionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceSearchRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+        "CollectionId": str,
+    },
+)
+_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceSearchRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "FaceMatchThreshold": float,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartFaceSearchRequestRequestTypeDef(
+    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
+):
+    pass
+
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetEntriesRequestRequestTypeDef",
+    {
+        "DatasetArn": str,
+        "Changes": DatasetChangesTypeDef,
+    },
+)
+
 _RequiredCompareFacesRequestRequestTypeDef = TypedDict(
     "_RequiredCompareFacesRequestRequestTypeDef",
     {
         "SourceImage": ImageTypeDef,
         "TargetImage": ImageTypeDef,
     },
 )
@@ -2776,145 +2955,14 @@
 
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
-_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartCelebrityRecognitionRequestRequestTypeDef(
-    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
-    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartContentModerationRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartContentModerationRequestRequestTypeDef",
-    {
-        "MinConfidence": float,
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartContentModerationRequestRequestTypeDef(
-    _RequiredStartContentModerationRequestRequestTypeDef,
-    _OptionalStartContentModerationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceDetectionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceDetectionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "FaceAttributes": FaceAttributesType,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartFaceDetectionRequestRequestTypeDef(
-    _RequiredStartFaceDetectionRequestRequestTypeDef,
-    _OptionalStartFaceDetectionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceSearchRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-        "CollectionId": str,
-    },
-)
-_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceSearchRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "FaceMatchThreshold": float,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartFaceSearchRequestRequestTypeDef(
-    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
-):
-    pass
-
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
 CelebrityTypeDef = TypedDict(
     "CelebrityTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Face": ComparedFaceTypeDef,
@@ -2942,15 +2990,15 @@
         "ModerationLabels": List[ContentModerationDetectionTypeDef],
         "NextToken": str,
         "ModerationModelVersion": str,
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectiveEquipmentBodyPartTypeDef = TypedDict(
     "ProtectiveEquipmentBodyPartTypeDef",
     {
         "Name": BodyPartType,
@@ -2970,33 +3018,33 @@
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetLabelsResponseTypeDef = TypedDict(
     "ListDatasetLabelsResponseTypeDef",
     {
         "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProjectsResponseTypeDef = TypedDict(
     "DescribeProjectsResponseTypeDef",
     {
         "ProjectDescriptions": List[ProjectDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectLabelsImagePropertiesTypeDef = TypedDict(
     "DetectLabelsImagePropertiesTypeDef",
     {
         "Quality": DetectLabelsImageQualityTypeDef,
@@ -3082,15 +3130,15 @@
 )
 
 DetectFacesResponseTypeDef = TypedDict(
     "DetectFacesResponseTypeDef",
     {
         "FaceDetails": List[FaceDetailTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FaceDetectionTypeDef = TypedDict(
     "FaceDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3140,14 +3188,17 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
+StreamProcessorSettingsUnionTypeDef = Union[
+    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
+]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3172,46 +3223,24 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3253,64 +3282,36 @@
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsTypeDef,
+        "Settings": StreamProcessorSettingsOutputTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestTypeDef],
+        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
@@ -3319,48 +3320,65 @@
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesByImageResponseTypeDef = TypedDict(
     "SearchFacesByImageResponseTypeDef",
     {
         "SearchedFaceBoundingBox": BoundingBoxTypeDef,
         "SearchedFaceConfidence": float,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesResponseTypeDef = TypedDict(
     "SearchFacesResponseTypeDef",
     {
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestingDataOutputTypeDef = TypedDict(
+    "TestingDataOutputTypeDef",
+    {
+        "Assets": List[AssetTypeDef],
+        "AutoCreate": bool,
     },
+    total=False,
 )
 
 TestingDataTypeDef = TypedDict(
     "TestingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
+TrainingDataOutputTypeDef = TypedDict(
+    "TrainingDataOutputTypeDef",
+    {
+        "Assets": List[AssetTypeDef],
+    },
+    total=False,
+)
+
 TrainingDataTypeDef = TypedDict(
     "TrainingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
@@ -3419,27 +3437,27 @@
 
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompareFacesResponseTypeDef = TypedDict(
     "CompareFacesResponseTypeDef",
     {
         "SourceImageFace": ComparedSourceImageFaceTypeDef,
         "FaceMatches": List[CompareFacesMatchTypeDef],
         "UnmatchedFaces": List[ComparedFaceTypeDef],
         "SourceImageOrientationCorrection": OrientationCorrectionType,
         "TargetImageOrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
@@ -3453,15 +3471,15 @@
 DetectLabelsResponseTypeDef = TypedDict(
     "DetectLabelsResponseTypeDef",
     {
         "Labels": List[LabelTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "LabelModelVersion": str,
         "ImageProperties": DetectLabelsImagePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3489,15 +3507,15 @@
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3519,43 +3537,43 @@
 IndexFacesResponseTypeDef = TypedDict(
     "IndexFacesResponseTypeDef",
     {
         "FaceRecords": List[FaceRecordTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "FaceModelVersion": str,
         "UnindexedFaces": List[UnindexedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchUsersByImageResponseTypeDef = TypedDict(
     "SearchUsersByImageResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceDetailsTypeDef,
         "UnsearchedFaces": List[UnsearchedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectCustomLabelsResponseTypeDef = TypedDict(
     "DetectCustomLabelsResponseTypeDef",
     {
         "CustomLabels": List[CustomLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectTextResponseTypeDef = TypedDict(
     "DetectTextResponseTypeDef",
     {
         "TextDetections": List[TextDetectionTypeDef],
         "TextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TextDetectionResultTypeDef = TypedDict(
     "TextDetectionResultTypeDef",
     {
         "Timestamp": int,
@@ -3579,14 +3597,65 @@
 )
 
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3602,14 +3671,15 @@
 
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
+TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3627,41 +3697,42 @@
 
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
+TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataTypeDef,
-        "Output": TestingDataTypeDef,
+        "Input": TestingDataOutputTypeDef,
+        "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataTypeDef,
-        "Output": TrainingDataTypeDef,
+        "Input": TrainingDataOutputTypeDef,
+        "Output": TrainingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
     {
         "ProtectiveEquipmentModelVersion": str,
         "Persons": List[ProtectiveEquipmentPersonTypeDef],
         "Summary": ProtectiveEquipmentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLabelDetectionResponseTypeDef = TypedDict(
     "GetLabelDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
@@ -3670,60 +3741,60 @@
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
     "GetCelebrityRecognitionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
@@ -3731,15 +3802,15 @@
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
         "JobId": str,
         "Video": VideoTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
@@ -3762,10 +3833,10 @@
 )
 
 DescribeProjectVersionsResponseTypeDef = TypedDict(
     "DescribeProjectVersionsResponseTypeDef",
     {
         "ProjectVersionDescriptions": List[ProjectVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/waiter.py` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition/waiter.pyi` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/PKG-INFO` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rekognition
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Rekognition 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Rekognition 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore rekognition type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore rekognition type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rekognition"></a>
 
 # types-aiobotocore-rekognition
 
 [![PyPI - types-aiobotocore-rekognition](https://img.shields.io/pypi/v/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rekognition?color=blue)](https://pypistats.org/packages/types-aiobotocore-rekognition)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Rekognition 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [types-aiobotocore-rekognition docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -416,79 +415,69 @@
 )
 
 
 def check_value(value: AttributeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_rekognition.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
+    ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
     BoundingBoxTypeDef,
     S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BlobTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
+    ConnectedHomeSettingsOutputTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
-    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
     LivenessOutputConfigTypeDef,
-    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
-    CreateStreamProcessorResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
-    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
-    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
-    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
@@ -526,100 +515,113 @@
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    PaginatorConfigTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
-    PutProjectPolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
+    StartShotDetectionFilterTypeDef,
+    StreamProcessingStopSelectorTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    CopyProjectVersionResponseTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    DeleteCollectionResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteProjectVersionResponseTypeDef,
+    DescribeCollectionResponseTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
-    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
-    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
     GroundTruthManifestTypeDef,
-    ImageTypeDef,
     SummaryTypeDef,
     VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
+    DatasetChangesTypeDef,
+    ImageTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
     LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
+    RegionOfInterestOutputTypeDef,
     RegionOfInterestTypeDef,
     HumanLoopConfigTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
@@ -627,29 +629,30 @@
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
     AssetTypeDef,
     DatasetSourceTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     CompareFacesRequestRequestTypeDef,
     DetectCustomLabelsRequestRequestTypeDef,
     DetectFacesRequestRequestTypeDef,
     DetectProtectiveEquipmentRequestRequestTypeDef,
     IndexFacesRequestRequestTypeDef,
     RecognizeCelebritiesRequestRequestTypeDef,
     SearchFacesByImageRequestRequestTypeDef,
     SearchUsersByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
@@ -662,28 +665,30 @@
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
+    RegionOfInterestUnionTypeDef,
     StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
-    CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    TestingDataOutputTypeDef,
     TestingDataTypeDef,
+    TrainingDataOutputTypeDef,
     TrainingDataTypeDef,
     ValidationDataTypeDef,
     CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
@@ -695,30 +700,34 @@
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
+    CreateStreamProcessorRequestRequestTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    TestingDataUnionTypeDef,
     CreateProjectVersionRequestRequestTypeDef,
+    TrainingDataUnionTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
-def get_structure() -> AgeRangeTypeDef:
+def get_value() -> AgeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rekognition-2.5.2/types_aiobotocore_rekognition.egg-info/SOURCES.txt` & `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*


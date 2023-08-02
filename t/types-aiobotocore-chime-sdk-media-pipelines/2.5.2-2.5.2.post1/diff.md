# Comparing `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.5.2.tar.gz` & `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.tar` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.153780 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-07-08 01:43:19.153780 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:19.153780 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.153780 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38659 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38614 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:39.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.153780 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.681642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-08-02 14:51:57.677642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.681642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.673642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48594 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48535 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.677642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/LICENSE` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/PKG-INFO` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-media-pipelines
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-media-pipelines"></a>
 
 # types-aiobotocore-chime-sdk-media-pipelines
 
 [![PyPI - types-aiobotocore-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-media-pipelines)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMediaPipelines 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [types-aiobotocore-chime-sdk-media-pipelines docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/).
 
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
@@ -314,21 +313,21 @@
 )
 
 
 def check_value(value: ArtifactsConcatenationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_media_pipelines.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_media_pipelines.type_defs import (
     PostCallAnalyticsSettingsTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
@@ -339,25 +338,26 @@
     VideoConcatenationConfigurationTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    TimestampRangeTypeDef,
+    TimestampRangeOutputTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     PresenterOnlyConfigurationTypeDef,
     IssueDetectionConfigurationTypeDef,
+    KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
     RecordingStreamConfigurationTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
@@ -367,70 +367,92 @@
     ListTagsForResourceRequestRequestTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
+    AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
+    StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    FragmentSelectorTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    FragmentSelectorOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    TimestampRangeTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
+    StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    FragmentSelectorTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ArtifactsConfigurationTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
-    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     ConcatenationSourceTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
     MediaInsightsPipelineTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> PostCallAnalyticsSettingsTypeDef:
+def get_value() -> PostCallAnalyticsSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/README.md` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-chime-sdk-media-pipelines
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-media-pipelines"></a>
 
 # types-aiobotocore-chime-sdk-media-pipelines
 
 [![PyPI - types-aiobotocore-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-media-pipelines)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMediaPipelines 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [types-aiobotocore-chime-sdk-media-pipelines docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +72,15 @@
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
@@ -281,21 +313,21 @@
 )
 
 
 def check_value(value: ArtifactsConcatenationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_media_pipelines.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_media_pipelines.type_defs import (
     PostCallAnalyticsSettingsTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
@@ -306,25 +338,26 @@
     VideoConcatenationConfigurationTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    TimestampRangeTypeDef,
+    TimestampRangeOutputTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     PresenterOnlyConfigurationTypeDef,
     IssueDetectionConfigurationTypeDef,
+    KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
     RecordingStreamConfigurationTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
@@ -334,70 +367,92 @@
     ListTagsForResourceRequestRequestTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
+    AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
+    StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    FragmentSelectorTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    FragmentSelectorOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    TimestampRangeTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
+    StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    FragmentSelectorTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ArtifactsConfigurationTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
-    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     ConcatenationSourceTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
     MediaInsightsPipelineTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> PostCallAnalyticsSettingsTypeDef:
+def get_value() -> PostCallAnalyticsSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/setup.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,46 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-media-pipelines",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "aiobotocore chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_media_pipelines": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/",
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/__init__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/__main__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/client.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,71 +18,67 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
-    LiveConnectorSourceConfigurationTypeDef,
-    MediaInsightsPipelineConfigurationElementTypeDef,
-    RealTimeAlertConfigurationTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ChimeSDKMediaPipelinesClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottledClientException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
 
-
 class ChimeSDKMediaPipelinesClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/)
     """
 
     meta: ClientMeta
@@ -91,270 +87,246 @@
     def exceptions(self) -> Exceptions:
         """
         ChimeSDKMediaPipelinesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#close)
         """
-
     async def create_media_capture_pipeline(
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
         """
-
     async def create_media_concatenation_pipeline(
         self,
         *,
         Sources: Sequence[ConcatenationSourceTypeDef],
         Sinks: Sequence[ConcatenationSinkTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaConcatenationPipelineResponseTypeDef:
         """
         Creates a media concatenation pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
-
     async def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
-
     async def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
-
     async def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
+        Sources: Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_live_connector_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_live_connector_pipeline)
         """
-
     async def delete_media_capture_pipeline(
         self, *, MediaPipelineId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#delete_media_capture_pipeline)
         """
-
     async def delete_media_insights_pipeline_configuration(
         self, *, Identifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#delete_media_insights_pipeline_configuration)
         """
-
     async def delete_media_pipeline(self, *, MediaPipelineId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#delete_media_pipeline)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#generate_presigned_url)
         """
-
     async def get_media_capture_pipeline(
         self, *, MediaPipelineId: str
     ) -> GetMediaCapturePipelineResponseTypeDef:
         """
         Gets an existing media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#get_media_capture_pipeline)
         """
-
     async def get_media_insights_pipeline_configuration(
         self, *, Identifier: str
     ) -> GetMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Gets the configuration settings for a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#get_media_insights_pipeline_configuration)
         """
-
     async def get_media_pipeline(self, *, MediaPipelineId: str) -> GetMediaPipelineResponseTypeDef:
         """
         Gets an existing media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#get_media_pipeline)
         """
-
     async def list_media_capture_pipelines(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaCapturePipelinesResponseTypeDef:
         """
         Returns a list of media pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_capture_pipelines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_media_capture_pipelines)
         """
-
     async def list_media_insights_pipeline_configurations(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaInsightsPipelineConfigurationsResponseTypeDef:
         """
         Lists the available media insights pipeline configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_insights_pipeline_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_media_insights_pipeline_configurations)
         """
-
     async def list_media_pipelines(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaPipelinesResponseTypeDef:
         """
         Returns a list of media pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_pipelines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_media_pipelines)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceARN: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags available for a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_tags_for_resource)
         """
-
     async def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         The ARN of the media pipeline that you want to tag.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes any tags from a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#untag_resource)
         """
-
     async def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
-
     async def update_media_insights_pipeline_status(
         self, *, Identifier: str, UpdateStatus: MediaPipelineStatusUpdateType
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the status of a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_status)
         """
-
     async def __aenter__(self) -> "ChimeSDKMediaPipelinesClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/)
         """
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/client.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,67 +18,71 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
-    LiveConnectorSourceConfigurationTypeDef,
-    MediaInsightsPipelineConfigurationElementTypeDef,
-    RealTimeAlertConfigurationTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ChimeSDKMediaPipelinesClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottledClientException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
 
+
 class ChimeSDKMediaPipelinesClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/)
     """
 
     meta: ClientMeta
@@ -87,246 +91,270 @@
     def exceptions(self) -> Exceptions:
         """
         ChimeSDKMediaPipelinesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#close)
         """
+
     async def create_media_capture_pipeline(
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
         """
+
     async def create_media_concatenation_pipeline(
         self,
         *,
         Sources: Sequence[ConcatenationSourceTypeDef],
         Sinks: Sequence[ConcatenationSinkTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaConcatenationPipelineResponseTypeDef:
         """
         Creates a media concatenation pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
+
     async def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
+
     async def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
+
     async def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
+        Sources: Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_live_connector_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_live_connector_pipeline)
         """
+
     async def delete_media_capture_pipeline(
         self, *, MediaPipelineId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#delete_media_capture_pipeline)
         """
+
     async def delete_media_insights_pipeline_configuration(
         self, *, Identifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#delete_media_insights_pipeline_configuration)
         """
+
     async def delete_media_pipeline(self, *, MediaPipelineId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#delete_media_pipeline)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#generate_presigned_url)
         """
+
     async def get_media_capture_pipeline(
         self, *, MediaPipelineId: str
     ) -> GetMediaCapturePipelineResponseTypeDef:
         """
         Gets an existing media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#get_media_capture_pipeline)
         """
+
     async def get_media_insights_pipeline_configuration(
         self, *, Identifier: str
     ) -> GetMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Gets the configuration settings for a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#get_media_insights_pipeline_configuration)
         """
+
     async def get_media_pipeline(self, *, MediaPipelineId: str) -> GetMediaPipelineResponseTypeDef:
         """
         Gets an existing media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#get_media_pipeline)
         """
+
     async def list_media_capture_pipelines(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaCapturePipelinesResponseTypeDef:
         """
         Returns a list of media pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_capture_pipelines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_media_capture_pipelines)
         """
+
     async def list_media_insights_pipeline_configurations(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaInsightsPipelineConfigurationsResponseTypeDef:
         """
         Lists the available media insights pipeline configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_insights_pipeline_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_media_insights_pipeline_configurations)
         """
+
     async def list_media_pipelines(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaPipelinesResponseTypeDef:
         """
         Returns a list of media pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_pipelines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_media_pipelines)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceARN: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags available for a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#list_tags_for_resource)
         """
+
     async def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         The ARN of the media pipeline that you want to tag.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes any tags from a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#untag_resource)
         """
+
     async def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
+
     async def update_media_insights_pipeline_status(
         self, *, Identifier: str, UpdateStatus: MediaPipelineStatusUpdateType
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the status of a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_status)
         """
+
     async def __aenter__(self) -> "ChimeSDKMediaPipelinesClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/)
         """
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/literals.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
 
-    data: PostCallAnalyticsSettingsTypeDef = {...}
+    data: PostCallAnalyticsSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -60,25 +60,26 @@
     "VideoConcatenationConfigurationTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "ChannelDefinitionTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "TimestampRangeTypeDef",
+    "TimestampRangeOutputTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "IssueDetectionConfigurationTypeDef",
+    "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
     "RecordingStreamConfigurationTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
@@ -88,65 +89,87 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
+    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
+    "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "FragmentSelectorTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "FragmentSelectorOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
+    "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "TimestampRangeTypeDef",
+    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
+    "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
+    "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
+    "FragmentSelectorTypeDef",
+    "MediaInsightsPipelineConfigurationElementUnionTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     "ArtifactsConfigurationTypeDef",
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
-    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
+    "RealTimeAlertConfigurationUnionTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "ConcatenationSourceTypeDef",
-    "CreateMediaInsightsPipelineRequestRequestTypeDef",
     "MediaInsightsPipelineTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
+    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
+    "LiveConnectorSourceConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
@@ -331,14 +354,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -360,26 +394,19 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
+TimestampRangeOutputTypeDef = TypedDict(
+    "TimestampRangeOutputTypeDef",
     {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": datetime,
+        "EndTimestamp": datetime,
     },
 )
 
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "GetMediaCapturePipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
@@ -411,14 +438,36 @@
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
+_RequiredKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKeywordMatchConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+        "Keywords": List[str],
+    },
+)
+_OptionalKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKeywordMatchConfigurationOutputTypeDef",
+    {
+        "Negate": bool,
+    },
+    total=False,
+)
+
+
+class KeywordMatchConfigurationOutputTypeDef(
+    _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -584,34 +633,33 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
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
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -620,14 +668,47 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
+_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "LanguageCode": CallAnalyticsLanguageCodeType,
+    },
+)
+_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "EnablePartialResultsStabilization": bool,
+        "PartialResultsStability": PartialResultsStabilityType,
+        "ContentIdentificationType": Literal["PII"],
+        "ContentRedactionType": Literal["PII"],
+        "PiiEntityTypes": str,
+        "FilterPartialResults": bool,
+        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
+        "CallAnalyticsStreamCategories": List[str],
+    },
+    total=False,
+)
+
+
+class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
+    _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+    _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -666,14 +747,35 @@
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
+_RequiredStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_RequiredStreamChannelDefinitionOutputTypeDef",
+    {
+        "NumberOfChannels": int,
+    },
+)
+_OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_OptionalStreamChannelDefinitionOutputTypeDef",
+    {
+        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+    },
+    total=False,
+)
+
+
+class StreamChannelDefinitionOutputTypeDef(
+    _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
+):
+    pass
+
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
@@ -695,35 +797,42 @@
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FragmentSelectorOutputTypeDef = TypedDict(
+    "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
+        "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
 
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
@@ -745,46 +854,69 @@
 
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
+_RequiredRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_RequiredRealTimeAlertRuleOutputTypeDef",
+    {
+        "Type": RealTimeAlertRuleTypeType,
+    },
+)
+_OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_OptionalRealTimeAlertRuleOutputTypeDef",
+    {
+        "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
+        "SentimentConfiguration": SentimentConfigurationTypeDef,
+        "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class RealTimeAlertRuleOutputTypeDef(
+    _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -800,22 +932,69 @@
 
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
 
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
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
+_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
+        "Type": MediaInsightsPipelineConfigurationElementTypeType,
+    },
+)
+_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
+        "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
+            AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
+        ),
+        "AmazonTranscribeProcessorConfiguration": AmazonTranscribeProcessorConfigurationTypeDef,
+        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationTypeDef,
+        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationTypeDef,
+        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationTypeDef,
+        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
+        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
+        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class MediaInsightsPipelineConfigurationElementOutputTypeDef(
+    _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
+    _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
+):
+    pass
+
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -846,14 +1025,36 @@
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
+_RequiredStreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+        "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
+    },
+)
+_OptionalStreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamConfigurationOutputTypeDef",
+    {
+        "FragmentNumber": str,
+    },
+    total=False,
+)
+
+
+class StreamConfigurationOutputTypeDef(
+    _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -868,19 +1069,19 @@
 
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
-        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorTypeDef,
+        "Streams": List[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
 
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
@@ -899,31 +1100,61 @@
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
 
+RealTimeAlertConfigurationOutputTypeDef = TypedDict(
+    "RealTimeAlertConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "Rules": List[RealTimeAlertRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
+MediaInsightsPipelineConfigurationElementUnionTypeDef = Union[
+    MediaInsightsPipelineConfigurationElementTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
+]
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
 
+KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
+    {
+        "Streams": List[StreamConfigurationOutputTypeDef],
+        "MediaEncoding": Literal["pcm"],
+        "MediaSampleRate": int,
+    },
+)
+
 KinesisVideoStreamSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
@@ -948,14 +1179,38 @@
 
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
 
+_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
+        "Arn": str,
+        "MuxType": LiveConnectorMuxTypeType,
+    },
+)
+_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
+        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
+    _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+    _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -972,20 +1227,46 @@
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
 
+MediaInsightsPipelineConfigurationTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationName": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "ResourceAccessRoleArn": str,
+        "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
+        "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
+        "MediaInsightsPipelineConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+RealTimeAlertConfigurationUnionTypeDef = Union[
+    RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+]
+KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    {
+        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorTypeDef,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
@@ -998,35 +1279,20 @@
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-MediaInsightsPipelineConfigurationTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationName": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "ResourceAccessRoleArn": str,
-        "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
-        "Elements": List[MediaInsightsPipelineConfigurationElementTypeDef],
-        "MediaInsightsPipelineConfigurationId": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
@@ -1045,108 +1311,135 @@
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
 
-_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationArn": str,
-    },
-)
-_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Mapping[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
-        ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class CreateMediaInsightsPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
-):
-    pass
-
-
 MediaInsightsPipelineTypeDef = TypedDict(
     "MediaInsightsPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "Status": MediaPipelineStatusType,
         "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
         ),
         "MediaInsightsRuntimeMetadata": Dict[str, str],
         "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
         ),
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
+]
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
+    },
+    total=False,
+)
+
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
+LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorSourceConfigurationOutputTypeDef",
+    {
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "ChimeSdkMeetingLiveConnectorConfiguration": (
+            ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
+        ),
+    },
+)
+
 LiveConnectorSourceConfigurationTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationTypeDef
         ),
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationArn": str,
+    },
+)
+_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Mapping[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
     },
+    total=False,
 )
 
+
+class CreateMediaInsightsPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
+):
+    pass
+
+
+KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
+]
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1181,143 +1474,149 @@
     total=False,
 )
 
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
-    {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateMediaCapturePipelineRequestRequestTypeDef(
-    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
-    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
-):
-    pass
-
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
+_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
-        "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
-        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
     },
 )
-_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+class CreateMediaCapturePipelineRequestRequestTypeDef(
+    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
+    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
 
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
-        "Sources": List[LiveConnectorSourceConfigurationTypeDef],
+        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+LiveConnectorSourceConfigurationUnionTypeDef = Union[
+    LiveConnectorSourceConfigurationTypeDef, LiveConnectorSourceConfigurationOutputTypeDef
+]
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "Sources": Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
+        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
+    },
+)
+_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+):
+    pass
+
+
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
 
-    data: PostCallAnalyticsSettingsTypeDef = {...}
+    data: PostCallAnalyticsSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -59,25 +59,26 @@
     "VideoConcatenationConfigurationTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "ChannelDefinitionTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "TimestampRangeTypeDef",
+    "TimestampRangeOutputTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "IssueDetectionConfigurationTypeDef",
+    "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
     "RecordingStreamConfigurationTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
@@ -87,65 +88,87 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
+    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
+    "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "FragmentSelectorTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "FragmentSelectorOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
+    "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "TimestampRangeTypeDef",
+    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
+    "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
+    "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
+    "FragmentSelectorTypeDef",
+    "MediaInsightsPipelineConfigurationElementUnionTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     "ArtifactsConfigurationTypeDef",
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
-    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
+    "RealTimeAlertConfigurationUnionTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "ConcatenationSourceTypeDef",
-    "CreateMediaInsightsPipelineRequestRequestTypeDef",
     "MediaInsightsPipelineTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
+    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
+    "LiveConnectorSourceConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
@@ -320,14 +343,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -349,26 +383,19 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
+TimestampRangeOutputTypeDef = TypedDict(
+    "TimestampRangeOutputTypeDef",
     {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": datetime,
+        "EndTimestamp": datetime,
     },
 )
 
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "GetMediaCapturePipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
@@ -400,14 +427,34 @@
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
+_RequiredKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKeywordMatchConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+        "Keywords": List[str],
+    },
+)
+_OptionalKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKeywordMatchConfigurationOutputTypeDef",
+    {
+        "Negate": bool,
+    },
+    total=False,
+)
+
+class KeywordMatchConfigurationOutputTypeDef(
+    _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -569,34 +616,33 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
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
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -605,14 +651,45 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
+_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "LanguageCode": CallAnalyticsLanguageCodeType,
+    },
+)
+_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "EnablePartialResultsStabilization": bool,
+        "PartialResultsStability": PartialResultsStabilityType,
+        "ContentIdentificationType": Literal["PII"],
+        "ContentRedactionType": Literal["PII"],
+        "PiiEntityTypes": str,
+        "FilterPartialResults": bool,
+        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
+        "CallAnalyticsStreamCategories": List[str],
+    },
+    total=False,
+)
+
+class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
+    _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+    _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -649,14 +726,33 @@
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
+_RequiredStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_RequiredStreamChannelDefinitionOutputTypeDef",
+    {
+        "NumberOfChannels": int,
+    },
+)
+_OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_OptionalStreamChannelDefinitionOutputTypeDef",
+    {
+        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+    },
+    total=False,
+)
+
+class StreamChannelDefinitionOutputTypeDef(
+    _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
+):
+    pass
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
@@ -676,35 +772,42 @@
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FragmentSelectorOutputTypeDef = TypedDict(
+    "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
+        "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
 
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
@@ -724,46 +827,67 @@
     pass
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
+_RequiredRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_RequiredRealTimeAlertRuleOutputTypeDef",
+    {
+        "Type": RealTimeAlertRuleTypeType,
+    },
+)
+_OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_OptionalRealTimeAlertRuleOutputTypeDef",
+    {
+        "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
+        "SentimentConfiguration": SentimentConfigurationTypeDef,
+        "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class RealTimeAlertRuleOutputTypeDef(
+    _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
+):
+    pass
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -777,22 +901,67 @@
 )
 
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
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
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
+_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
+        "Type": MediaInsightsPipelineConfigurationElementTypeType,
+    },
+)
+_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
+        "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
+            AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
+        ),
+        "AmazonTranscribeProcessorConfiguration": AmazonTranscribeProcessorConfigurationTypeDef,
+        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationTypeDef,
+        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationTypeDef,
+        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationTypeDef,
+        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
+        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
+        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class MediaInsightsPipelineConfigurationElementOutputTypeDef(
+    _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
+    _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
+):
+    pass
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -821,14 +990,34 @@
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
+_RequiredStreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+        "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
+    },
+)
+_OptionalStreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamConfigurationOutputTypeDef",
+    {
+        "FragmentNumber": str,
+    },
+    total=False,
+)
+
+class StreamConfigurationOutputTypeDef(
+    _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -841,19 +1030,19 @@
 )
 
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
-        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorTypeDef,
+        "Streams": List[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
 
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
@@ -870,31 +1059,61 @@
 
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
+RealTimeAlertConfigurationOutputTypeDef = TypedDict(
+    "RealTimeAlertConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "Rules": List[RealTimeAlertRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
+MediaInsightsPipelineConfigurationElementUnionTypeDef = Union[
+    MediaInsightsPipelineConfigurationElementTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
+]
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
 
+KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
+    {
+        "Streams": List[StreamConfigurationOutputTypeDef],
+        "MediaEncoding": Literal["pcm"],
+        "MediaSampleRate": int,
+    },
+)
+
 KinesisVideoStreamSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
@@ -917,14 +1136,36 @@
 )
 
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
+_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
+        "Arn": str,
+        "MuxType": LiveConnectorMuxTypeType,
+    },
+)
+_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
+        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
+    _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+    _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -939,20 +1180,46 @@
 
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
+MediaInsightsPipelineConfigurationTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationName": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "ResourceAccessRoleArn": str,
+        "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
+        "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
+        "MediaInsightsPipelineConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+RealTimeAlertConfigurationUnionTypeDef = Union[
+    RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+]
+KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    {
+        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorTypeDef,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
@@ -963,35 +1230,20 @@
 
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-MediaInsightsPipelineConfigurationTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationName": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "ResourceAccessRoleArn": str,
-        "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
-        "Elements": List[MediaInsightsPipelineConfigurationElementTypeDef],
-        "MediaInsightsPipelineConfigurationId": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
@@ -1008,106 +1260,133 @@
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
 
-_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationArn": str,
-    },
-)
-_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Mapping[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
-        ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-class CreateMediaInsightsPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
-):
-    pass
-
 MediaInsightsPipelineTypeDef = TypedDict(
     "MediaInsightsPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "Status": MediaPipelineStatusType,
         "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
         ),
         "MediaInsightsRuntimeMetadata": Dict[str, str],
         "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
         ),
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
+]
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
+    },
+    total=False,
+)
+
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
+LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorSourceConfigurationOutputTypeDef",
+    {
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "ChimeSdkMeetingLiveConnectorConfiguration": (
+            ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
+        ),
+    },
+)
+
 LiveConnectorSourceConfigurationTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationTypeDef
         ),
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationArn": str,
+    },
+)
+_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Mapping[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class CreateMediaInsightsPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
+):
+    pass
+
+KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
+]
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1140,139 +1419,145 @@
     total=False,
 )
 
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
-    {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-    },
-)
-_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateMediaCapturePipelineRequestRequestTypeDef(
-    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
-    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
-):
-    pass
-
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
+_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
-        "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
-        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
     },
 )
-_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+class CreateMediaCapturePipelineRequestRequestTypeDef(
+    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
+    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
-        "Sources": List[LiveConnectorSourceConfigurationTypeDef],
+        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+LiveConnectorSourceConfigurationUnionTypeDef = Union[
+    LiveConnectorSourceConfigurationTypeDef, LiveConnectorSourceConfigurationOutputTypeDef
+]
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "Sources": Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
+        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
+    },
+)
+_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+):
+    pass
+
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-chime-sdk-media-pipelines
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-media-pipelines"></a>
 
 # types-aiobotocore-chime-sdk-media-pipelines
 
 [![PyPI - types-aiobotocore-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-media-pipelines)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMediaPipelines 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [types-aiobotocore-chime-sdk-media-pipelines docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +40,15 @@
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
@@ -314,21 +281,21 @@
 )
 
 
 def check_value(value: ArtifactsConcatenationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_media_pipelines.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_media_pipelines.type_defs import (
     PostCallAnalyticsSettingsTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
@@ -339,25 +306,26 @@
     VideoConcatenationConfigurationTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    TimestampRangeTypeDef,
+    TimestampRangeOutputTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     PresenterOnlyConfigurationTypeDef,
     IssueDetectionConfigurationTypeDef,
+    KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
     RecordingStreamConfigurationTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
@@ -367,70 +335,92 @@
     ListTagsForResourceRequestRequestTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
+    AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
+    StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    FragmentSelectorTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    FragmentSelectorOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    TimestampRangeTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
+    StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    FragmentSelectorTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ArtifactsConfigurationTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
-    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     ConcatenationSourceTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
     MediaInsightsPipelineTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> PostCallAnalyticsSettingsTypeDef:
+def get_value() -> PostCallAnalyticsSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*


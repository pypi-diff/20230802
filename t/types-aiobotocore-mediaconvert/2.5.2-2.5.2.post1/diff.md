# Comparing `tmp/types-aiobotocore-mediaconvert-2.5.2.tar.gz` & `tmp/types-aiobotocore-mediaconvert-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconvert-2.5.2.tar", last modified: Sat Jul  8 01:43:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconvert-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
```

## Comparing `types-aiobotocore-mediaconvert-2.5.2.tar` & `types-aiobotocore-mediaconvert-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:58.034515 types-aiobotocore-mediaconvert-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33561 2023-07-08 01:43:58.034515 types-aiobotocore-mediaconvert-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31976 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:58.034515 types-aiobotocore-mediaconvert-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:58.034515 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24276 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-07-08 01:34:52.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55529 2023-07-08 01:34:51.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-08 01:34:51.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   103387 2023-07-08 01:34:55.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103362 2023-07-08 01:34:53.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:50.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:58.034515 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33561 2023-07-08 01:43:57.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:57.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:57.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:57.000000 types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35083 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33545 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24274 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-08-02 14:43:06.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55529 2023-08-02 14:43:05.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   127164 2023-08-02 14:43:08.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127139 2023-08-02 14:43:07.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35083 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/LICENSE` & `types-aiobotocore-mediaconvert-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2/PKG-INFO` & `types-aiobotocore-mediaconvert-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconvert
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore mediaconvert type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mediaconvert"></a>
 
 # types-aiobotocore-mediaconvert
 
 [![PyPI - types-aiobotocore-mediaconvert](https://img.shields.io/pypi/v/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mediaconvert?color=blue)](https://pypistats.org/packages/types-aiobotocore-mediaconvert)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MediaConvert 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [types-aiobotocore-mediaconvert docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/).
 
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
@@ -731,20 +730,20 @@
 )
 
 
 def check_value(value: AacAudioDescriptionBroadcasterMixType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mediaconvert.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mediaconvert.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AccelerationSettingsTypeDef,
     AdvancedInputFilterSettingsTypeDef,
@@ -757,14 +756,15 @@
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
     HlsRenditionGroupSettingsTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
     Av1QvbrSettingsTypeDef,
     AvailBlankingTypeDef,
@@ -773,46 +773,54 @@
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
-    TeletextDestinationSettingsTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    TeletextDestinationSettingsTypeDef,
     CaptionSourceFramerateTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
+    OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
     ClipLimitsTypeDef,
+    CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
-    SpekeKeyProviderCmafTypeDef,
+    SpekeKeyProviderCmafOutputTypeDef,
     StaticKeyProviderTypeDef,
+    SpekeKeyProviderCmafTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
     CmfcSettingsTypeDef,
     Hdr10MetadataTypeDef,
     F4vSettingsTypeDef,
-    M3u8SettingsTypeDef,
+    M3u8SettingsOutputTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
+    M3u8SettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
+    DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
@@ -824,161 +832,195 @@
     GetJobTemplateRequestRequestTypeDef,
     PolicyTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
     H264QvbrSettingsTypeDef,
     H265QvbrSettingsTypeDef,
     Hdr10PlusTypeDef,
+    HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
     HlsCaptionLanguageMappingTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
     HlsSettingsTypeDef,
     Id3InsertionTypeDef,
     InsertableImageTypeDef,
     InputClippingTypeDef,
     InputDecryptionSettingsTypeDef,
-    RectangleTypeDef,
     InputVideoGeneratorTypeDef,
+    RectangleTypeDef,
     JobMessagesTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
     Mpeg2SettingsTypeDef,
+    MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
     MxfXavcProfileSettingsTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
     Vc3SettingsTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
     Xavc4kProfileSettingsTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
     XavcHdProfileSettingsTypeDef,
     AudioCodecSettingsTypeDef,
+    AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
     Av1SettingsTypeDef,
     AvcIntraSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
     FileSourceSettingsTypeDef,
+    ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
+    CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
+    DashIsoEncryptionSettingsOutputTypeDef,
+    HlsEncryptionSettingsOutputTypeDef,
+    MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
     H264SettingsTypeDef,
     H265SettingsTypeDef,
     OutputSettingsTypeDef,
+    TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
+    ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
+    M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
     MotionImageInserterTypeDef,
     MxfSettingsTypeDef,
     PartnerWatermarkingTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
     QueueTypeDef,
     S3DestinationSettingsTypeDef,
     XavcSettingsTypeDef,
+    AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
     CaptionDescriptionTypeDef,
     CaptionSourceSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
+    VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
     DestinationSettingsTypeDef,
     VideoCodecSettingsTypeDef,
+    AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
     CaptionSelectorTypeDef,
+    AudioDescriptionOutputTypeDef,
+    AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
+    CmafGroupSettingsOutputTypeDef,
     CmafGroupSettingsTypeDef,
+    DashIsoGroupSettingsOutputTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
+    HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
+    InputOutputTypeDef,
+    InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
+    PresetSettingsOutputTypeDef,
     OutputTypeDef,
     PresetSettingsTypeDef,
+    PresetTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
     CreatePresetRequestRequestTypeDef,
-    PresetTypeDef,
+    PresetSettingsUnionTypeDef,
     UpdatePresetRequestRequestTypeDef,
-    JobSettingsTypeDef,
-    JobTemplateSettingsTypeDef,
     CreatePresetResponseTypeDef,
     GetPresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     UpdatePresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
+    JobSettingsOutputTypeDef,
+    JobTemplateSettingsOutputTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     JobTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobRequestRequestTypeDef,
+    JobSettingsUnionTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
+    JobTemplateSettingsUnionTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_value() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/README.md` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-mediaconvert
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore mediaconvert type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mediaconvert"></a>
 
 # types-aiobotocore-mediaconvert
 
 [![PyPI - types-aiobotocore-mediaconvert](https://img.shields.io/pypi/v/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mediaconvert?color=blue)](https://pypistats.org/packages/types-aiobotocore-mediaconvert)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MediaConvert 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [types-aiobotocore-mediaconvert docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/).
 
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
@@ -698,20 +730,20 @@
 )
 
 
 def check_value(value: AacAudioDescriptionBroadcasterMixType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mediaconvert.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mediaconvert.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AccelerationSettingsTypeDef,
     AdvancedInputFilterSettingsTypeDef,
@@ -724,14 +756,15 @@
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
     HlsRenditionGroupSettingsTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
     Av1QvbrSettingsTypeDef,
     AvailBlankingTypeDef,
@@ -740,46 +773,54 @@
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
-    TeletextDestinationSettingsTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    TeletextDestinationSettingsTypeDef,
     CaptionSourceFramerateTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
+    OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
     ClipLimitsTypeDef,
+    CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
-    SpekeKeyProviderCmafTypeDef,
+    SpekeKeyProviderCmafOutputTypeDef,
     StaticKeyProviderTypeDef,
+    SpekeKeyProviderCmafTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
     CmfcSettingsTypeDef,
     Hdr10MetadataTypeDef,
     F4vSettingsTypeDef,
-    M3u8SettingsTypeDef,
+    M3u8SettingsOutputTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
+    M3u8SettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
+    DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
@@ -791,161 +832,195 @@
     GetJobTemplateRequestRequestTypeDef,
     PolicyTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
     H264QvbrSettingsTypeDef,
     H265QvbrSettingsTypeDef,
     Hdr10PlusTypeDef,
+    HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
     HlsCaptionLanguageMappingTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
     HlsSettingsTypeDef,
     Id3InsertionTypeDef,
     InsertableImageTypeDef,
     InputClippingTypeDef,
     InputDecryptionSettingsTypeDef,
-    RectangleTypeDef,
     InputVideoGeneratorTypeDef,
+    RectangleTypeDef,
     JobMessagesTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
     Mpeg2SettingsTypeDef,
+    MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
     MxfXavcProfileSettingsTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
     Vc3SettingsTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
     Xavc4kProfileSettingsTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
     XavcHdProfileSettingsTypeDef,
     AudioCodecSettingsTypeDef,
+    AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
     Av1SettingsTypeDef,
     AvcIntraSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
     FileSourceSettingsTypeDef,
+    ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
+    CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
+    DashIsoEncryptionSettingsOutputTypeDef,
+    HlsEncryptionSettingsOutputTypeDef,
+    MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
     H264SettingsTypeDef,
     H265SettingsTypeDef,
     OutputSettingsTypeDef,
+    TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
+    ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
+    M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
     MotionImageInserterTypeDef,
     MxfSettingsTypeDef,
     PartnerWatermarkingTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
     QueueTypeDef,
     S3DestinationSettingsTypeDef,
     XavcSettingsTypeDef,
+    AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
     CaptionDescriptionTypeDef,
     CaptionSourceSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
+    VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
     DestinationSettingsTypeDef,
     VideoCodecSettingsTypeDef,
+    AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
     CaptionSelectorTypeDef,
+    AudioDescriptionOutputTypeDef,
+    AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
+    CmafGroupSettingsOutputTypeDef,
     CmafGroupSettingsTypeDef,
+    DashIsoGroupSettingsOutputTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
+    HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
+    InputOutputTypeDef,
+    InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
+    PresetSettingsOutputTypeDef,
     OutputTypeDef,
     PresetSettingsTypeDef,
+    PresetTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
     CreatePresetRequestRequestTypeDef,
-    PresetTypeDef,
+    PresetSettingsUnionTypeDef,
     UpdatePresetRequestRequestTypeDef,
-    JobSettingsTypeDef,
-    JobTemplateSettingsTypeDef,
     CreatePresetResponseTypeDef,
     GetPresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     UpdatePresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
+    JobSettingsOutputTypeDef,
+    JobTemplateSettingsOutputTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     JobTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobRequestRequestTypeDef,
+    JobSettingsUnionTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
+    JobTemplateSettingsUnionTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_value() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/setup.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconvert",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with"
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
-    keywords="aiobotocore mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore mediaconvert type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediaconvert": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/"
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/__init__.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/__init__.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/__main__.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConvert 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.MediaConvert 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
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

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/client.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,23 +49,23 @@
     DescribeEndpointsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetPresetResponseTypeDef,
     GetQueueResponseTypeDef,
     HopDestinationTypeDef,
-    JobSettingsTypeDef,
-    JobTemplateSettingsTypeDef,
+    JobSettingsUnionTypeDef,
+    JobTemplateSettingsUnionTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListPresetsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PolicyTypeDef,
-    PresetSettingsTypeDef,
+    PresetSettingsUnionTypeDef,
     PutPolicyResponseTypeDef,
     ReservationPlanSettingsTypeDef,
     UpdateJobTemplateResponseTypeDef,
     UpdatePresetResponseTypeDef,
     UpdateQueueResponseTypeDef,
 )
 
@@ -146,15 +146,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#close)
         """
 
     async def create_job(
         self,
         *,
         Role: str,
-        Settings: JobSettingsTypeDef,
+        Settings: JobSettingsUnionTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         BillingTagsSource: BillingTagsSourceType = ...,
         ClientRequestToken: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
@@ -170,15 +170,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job)
         """
 
     async def create_job_template(
         self,
         *,
         Name: str,
-        Settings: JobTemplateSettingsTypeDef,
+        Settings: JobTemplateSettingsUnionTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
@@ -191,15 +191,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job_template)
         """
 
     async def create_preset(
         self,
         *,
         Name: str,
-        Settings: PresetSettingsTypeDef,
+        Settings: PresetSettingsUnionTypeDef,
         Category: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
@@ -432,15 +432,15 @@
         Name: str,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
-        Settings: JobTemplateSettingsTypeDef = ...,
+        Settings: JobTemplateSettingsUnionTypeDef = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_job_template)
@@ -448,15 +448,15 @@
 
     async def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsTypeDef = ...
+        Settings: PresetSettingsUnionTypeDef = ...
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_preset)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/client.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -49,23 +49,23 @@
     DescribeEndpointsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetPresetResponseTypeDef,
     GetQueueResponseTypeDef,
     HopDestinationTypeDef,
-    JobSettingsTypeDef,
-    JobTemplateSettingsTypeDef,
+    JobSettingsUnionTypeDef,
+    JobTemplateSettingsUnionTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListPresetsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PolicyTypeDef,
-    PresetSettingsTypeDef,
+    PresetSettingsUnionTypeDef,
     PutPolicyResponseTypeDef,
     ReservationPlanSettingsTypeDef,
     UpdateJobTemplateResponseTypeDef,
     UpdatePresetResponseTypeDef,
     UpdateQueueResponseTypeDef,
 )
 
@@ -137,15 +137,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#close)
         """
     async def create_job(
         self,
         *,
         Role: str,
-        Settings: JobSettingsTypeDef,
+        Settings: JobSettingsUnionTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         BillingTagsSource: BillingTagsSourceType = ...,
         ClientRequestToken: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
@@ -160,15 +160,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job)
         """
     async def create_job_template(
         self,
         *,
         Name: str,
-        Settings: JobTemplateSettingsTypeDef,
+        Settings: JobTemplateSettingsUnionTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
@@ -180,15 +180,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job_template)
         """
     async def create_preset(
         self,
         *,
         Name: str,
-        Settings: PresetSettingsTypeDef,
+        Settings: PresetSettingsUnionTypeDef,
         Category: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
@@ -399,30 +399,30 @@
         Name: str,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
-        Settings: JobTemplateSettingsTypeDef = ...,
+        Settings: JobTemplateSettingsUnionTypeDef = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_job_template)
         """
     async def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsTypeDef = ...
+        Settings: PresetSettingsUnionTypeDef = ...
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_preset)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/literals.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/literals.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/paginator.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 
@@ -95,15 +95,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -115,15 +115,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobspaginator)
         """
 
 
@@ -135,15 +135,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listpresetspaginator)
         """
 
 
@@ -154,13 +154,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/paginator.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 class ListJobTemplatesPaginator(AioPaginator):
@@ -91,15 +91,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(AioPaginator):
@@ -110,15 +110,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobspaginator)
         """
 
 class ListPresetsPaginator(AioPaginator):
@@ -129,15 +129,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listpresetspaginator)
         """
 
 class ListQueuesPaginator(AioPaginator):
@@ -147,13 +147,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/type_defs.py` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_mediaconvert.type_defs import AacSettingsTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AacAudioDescriptionBroadcasterMixType,
     AacCodecProfileType,
     AacCodingModeType,
     AacRateControlModeType,
     AacRawFormatType,
@@ -445,14 +445,15 @@
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
     "AudioNormalizationSettingsTypeDef",
+    "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
     "Av1QvbrSettingsTypeDef",
     "AvailBlankingTypeDef",
@@ -461,46 +462,54 @@
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsTypeDef",
+    "TeletextDestinationSettingsOutputTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
+    "TeletextDestinationSettingsTypeDef",
     "CaptionSourceFramerateTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
+    "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
     "ClipLimitsTypeDef",
+    "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
-    "SpekeKeyProviderCmafTypeDef",
+    "SpekeKeyProviderCmafOutputTypeDef",
     "StaticKeyProviderTypeDef",
+    "SpekeKeyProviderCmafTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
     "CmfcSettingsTypeDef",
     "Hdr10MetadataTypeDef",
     "F4vSettingsTypeDef",
-    "M3u8SettingsTypeDef",
+    "M3u8SettingsOutputTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
+    "M3u8SettingsTypeDef",
     "HopDestinationTypeDef",
+    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
+    "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
@@ -512,149 +521,183 @@
     "GetJobTemplateRequestRequestTypeDef",
     "PolicyTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
     "H264QvbrSettingsTypeDef",
     "H265QvbrSettingsTypeDef",
     "Hdr10PlusTypeDef",
+    "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
     "HlsSettingsTypeDef",
     "Id3InsertionTypeDef",
     "InsertableImageTypeDef",
     "InputClippingTypeDef",
     "InputDecryptionSettingsTypeDef",
-    "RectangleTypeDef",
     "InputVideoGeneratorTypeDef",
+    "RectangleTypeDef",
     "JobMessagesTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
     "Mpeg2SettingsTypeDef",
+    "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
     "MxfXavcProfileSettingsTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
-    "PaginatorConfigTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationAccessControlTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "Vc3SettingsTypeDef",
     "Vp8SettingsTypeDef",
     "Vp9SettingsTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     "Xavc4kProfileSettingsTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
     "XavcHdProfileSettingsTypeDef",
     "AudioCodecSettingsTypeDef",
+    "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
     "Av1SettingsTypeDef",
     "AvcIntraSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "FileSourceSettingsTypeDef",
+    "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
+    "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    "HlsEncryptionSettingsOutputTypeDef",
+    "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DolbyVisionTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
     "H264SettingsTypeDef",
     "H265SettingsTypeDef",
     "OutputSettingsTypeDef",
+    "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
+    "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
     "MotionImageInserterTypeDef",
     "MxfSettingsTypeDef",
     "PartnerWatermarkingTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
     "QueueTypeDef",
     "S3DestinationSettingsTypeDef",
     "XavcSettingsTypeDef",
+    "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
+    "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
     "CaptionDescriptionTypeDef",
     "CaptionSourceSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
+    "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
     "DestinationSettingsTypeDef",
     "VideoCodecSettingsTypeDef",
+    "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
     "CaptionSelectorTypeDef",
+    "AudioDescriptionOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
+    "CmafGroupSettingsOutputTypeDef",
     "CmafGroupSettingsTypeDef",
+    "DashIsoGroupSettingsOutputTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
     "MsSmoothGroupSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
+    "InputOutputTypeDef",
+    "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
+    "PresetSettingsOutputTypeDef",
     "OutputTypeDef",
     "PresetSettingsTypeDef",
+    "PresetTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "PresetTypeDef",
+    "PresetSettingsUnionTypeDef",
     "UpdatePresetRequestRequestTypeDef",
-    "JobSettingsTypeDef",
-    "JobTemplateSettingsTypeDef",
     "CreatePresetResponseTypeDef",
     "GetPresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "UpdatePresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
+    "JobSettingsOutputTypeDef",
+    "JobTemplateSettingsOutputTypeDef",
+    "JobSettingsTypeDef",
+    "JobTemplateSettingsTypeDef",
     "JobTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "JobSettingsUnionTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
+    "JobTemplateSettingsUnionTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
@@ -870,14 +913,22 @@
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
     total=False,
 )
 
+AudioSelectorGroupOutputTypeDef = TypedDict(
+    "AudioSelectorGroupOutputTypeDef",
+    {
+        "AudioSelectorNames": List[str],
+    },
+    total=False,
+)
+
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
@@ -1052,19 +1103,19 @@
     "SrtDestinationSettingsTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsTypeDef = TypedDict(
-    "TeletextDestinationSettingsTypeDef",
+TeletextDestinationSettingsOutputTypeDef = TypedDict(
+    "TeletextDestinationSettingsOutputTypeDef",
     {
         "PageNumber": str,
-        "PageTypes": Sequence[TeletextPageTypeType],
+        "PageTypes": List[TeletextPageTypeType],
     },
     total=False,
 )
 
 TtmlDestinationSettingsTypeDef = TypedDict(
     "TtmlDestinationSettingsTypeDef",
     {
@@ -1078,14 +1129,23 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
+TeletextDestinationSettingsTypeDef = TypedDict(
+    "TeletextDestinationSettingsTypeDef",
+    {
+        "PageNumber": str,
+        "PageTypes": Sequence[TeletextPageTypeType],
+    },
+    total=False,
+)
+
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -1132,14 +1192,23 @@
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+OutputChannelMappingOutputTypeDef = TypedDict(
+    "OutputChannelMappingOutputTypeDef",
+    {
+        "InputChannels": List[int],
+        "InputChannelsFineTune": List[float],
+    },
+    total=False,
+)
+
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
@@ -1152,29 +1221,38 @@
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
     total=False,
 )
 
+CmafAdditionalManifestOutputTypeDef = TypedDict(
+    "CmafAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
-SpekeKeyProviderCmafTypeDef = TypedDict(
-    "SpekeKeyProviderCmafTypeDef",
+SpekeKeyProviderCmafOutputTypeDef = TypedDict(
+    "SpekeKeyProviderCmafOutputTypeDef",
     {
         "CertificateArn": str,
-        "DashSignaledSystemIds": Sequence[str],
-        "HlsSignaledSystemIds": Sequence[str],
+        "DashSignaledSystemIds": List[str],
+        "HlsSignaledSystemIds": List[str],
         "ResourceId": str,
         "Url": str,
     },
     total=False,
 )
 
 StaticKeyProviderTypeDef = TypedDict(
@@ -1184,14 +1262,26 @@
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
     total=False,
 )
 
+SpekeKeyProviderCmafTypeDef = TypedDict(
+    "SpekeKeyProviderCmafTypeDef",
+    {
+        "CertificateArn": str,
+        "DashSignaledSystemIds": Sequence[str],
+        "HlsSignaledSystemIds": Sequence[str],
+        "ResourceId": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
@@ -1245,20 +1335,20 @@
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
     total=False,
 )
 
-M3u8SettingsTypeDef = TypedDict(
-    "M3u8SettingsTypeDef",
+M3u8SettingsOutputTypeDef = TypedDict(
+    "M3u8SettingsOutputTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
-        "AudioPids": Sequence[int],
+        "AudioPids": List[int],
         "DataPTSControl": M3u8DataPtsControlType,
         "MaxPcrInterval": int,
         "NielsenId3": M3u8NielsenId3Type,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
         "PcrPid": int,
         "PmtInterval": int,
@@ -1314,42 +1404,99 @@
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
+M3u8SettingsTypeDef = TypedDict(
+    "M3u8SettingsTypeDef",
+    {
+        "AudioDuration": M3u8AudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": Sequence[int],
+        "DataPTSControl": M3u8DataPtsControlType,
+        "MaxPcrInterval": int,
+        "NielsenId3": M3u8NielsenId3Type,
+        "PatInterval": int,
+        "PcrControl": M3u8PcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "Scte35Pid": int,
+        "Scte35Source": M3u8Scte35SourceType,
+        "TimedMetadata": TimedMetadataType,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
+    },
+    total=False,
+)
+
 HopDestinationTypeDef = TypedDict(
     "HopDestinationTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
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
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
 )
 
+DashAdditionalManifestOutputTypeDef = TypedDict(
+    "DashAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "ResourceId": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+    total=False,
+)
+
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -1397,19 +1544,20 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -1572,14 +1720,23 @@
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
 )
 
+HlsAdditionalManifestOutputTypeDef = TypedDict(
+    "HlsAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -1666,33 +1823,33 @@
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
+InputVideoGeneratorTypeDef = TypedDict(
+    "InputVideoGeneratorTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
     total=False,
 )
 
-InputVideoGeneratorTypeDef = TypedDict(
-    "InputVideoGeneratorTypeDef",
-    {
-        "Duration": int,
-    },
-    total=False,
-)
-
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
     total=False,
@@ -1780,93 +1937,50 @@
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
     },
 )
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -1952,14 +2066,23 @@
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
     total=False,
 )
 
+MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
+    "MsSmoothAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -2020,24 +2143,14 @@
     {
         "HeightInPx": int,
         "WidthInPx": int,
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
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -2063,25 +2176,14 @@
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
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
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
@@ -2260,14 +2362,26 @@
         "OpusSettings": OpusSettingsTypeDef,
         "VorbisSettings": VorbisSettingsTypeDef,
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrRuleOutputTypeDef = TypedDict(
+    "AutomatedAbrRuleOutputTypeDef",
+    {
+        "AllowedRenditions": List[AllowedRenditionSizeTypeDef],
+        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeTypeDef],
+        "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
+        "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
+        "Type": RuleTypeType,
+    },
+    total=False,
+)
+
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
@@ -2309,14 +2423,31 @@
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
     total=False,
 )
 
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
+        "DestinationType": CaptionDestinationTypeType,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
+        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
+        "ImscDestinationSettings": ImscDestinationSettingsTypeDef,
+        "SccDestinationSettings": SccDestinationSettingsTypeDef,
+        "SrtDestinationSettings": SrtDestinationSettingsTypeDef,
+        "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
+    },
+    total=False,
+)
+
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
@@ -2339,22 +2470,43 @@
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
 
+ChannelMappingOutputTypeDef = TypedDict(
+    "ChannelMappingOutputTypeDef",
+    {
+        "OutputChannels": List[OutputChannelMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
     total=False,
 )
 
+CmafEncryptionSettingsOutputTypeDef = TypedDict(
+    "CmafEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": CmafEncryptionTypeType,
+        "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
+        "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "Type": CmafKeyProviderTypeType,
+    },
+    total=False,
+)
+
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
@@ -2442,14 +2594,45 @@
 
 class UpdateQueueRequestRequestTypeDef(
     _RequiredUpdateQueueRequestRequestTypeDef, _OptionalUpdateQueueRequestRequestTypeDef
 ):
     pass
 
 
+DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    {
+        "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+    total=False,
+)
+
+HlsEncryptionSettingsOutputTypeDef = TypedDict(
+    "HlsEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": HlsEncryptionTypeType,
+        "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
+        "OfflineEncrypted": HlsOfflineEncryptedType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "Type": HlsKeyProviderTypeType,
+    },
+    total=False,
+)
+
+MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
+    "MsSmoothEncryptionSettingsOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+    total=False,
+)
+
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
@@ -2473,20 +2656,72 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    {
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
@@ -2507,30 +2742,30 @@
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPolicyRequestRequestTypeDef = TypedDict(
     "PutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2632,39 +2867,102 @@
     "OutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
     },
     total=False,
 )
 
+TimedMetadataInsertionOutputTypeDef = TypedDict(
+    "TimedMetadataInsertionOutputTypeDef",
+    {
+        "Id3Insertions": List[Id3InsertionTypeDef],
+    },
+    total=False,
+)
+
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
+ImageInserterOutputTypeDef = TypedDict(
+    "ImageInserterOutputTypeDef",
+    {
+        "InsertableImages": List[InsertableImageTypeDef],
+        "SdrReferenceWhiteLevel": int,
+    },
+    total=False,
+)
+
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+M2tsSettingsOutputTypeDef = TypedDict(
+    "M2tsSettingsOutputTypeDef",
+    {
+        "AudioBufferModel": M2tsAudioBufferModelType,
+        "AudioDuration": M2tsAudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": List[int],
+        "Bitrate": int,
+        "BufferModel": M2tsBufferModelType,
+        "DataPTSControl": M2tsDataPtsControlType,
+        "DvbNitSettings": DvbNitSettingsTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsTypeDef,
+        "DvbSubPids": List[int],
+        "DvbTdtSettings": DvbTdtSettingsTypeDef,
+        "DvbTeletextPid": int,
+        "EbpAudioInterval": M2tsEbpAudioIntervalType,
+        "EbpPlacement": M2tsEbpPlacementType,
+        "EsRateInPes": M2tsEsRateInPesType,
+        "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
+        "FragmentTime": float,
+        "KlvMetadata": M2tsKlvMetadataType,
+        "MaxPcrInterval": int,
+        "MinEbpInterval": int,
+        "NielsenId3": M2tsNielsenId3Type,
+        "NullPacketBitrate": float,
+        "PatInterval": int,
+        "PcrControl": M2tsPcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "RateMode": M2tsRateModeType,
+        "Scte35Esam": M2tsScte35EsamTypeDef,
+        "Scte35Pid": int,
+        "Scte35Source": M2tsScte35SourceType,
+        "SegmentationMarkers": M2tsSegmentationMarkersType,
+        "SegmentationStyle": M2tsSegmentationStyleType,
+        "SegmentationTime": float,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
+    },
+    total=False,
+)
+
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
         "AudioFramesPerPes": int,
         "AudioPids": Sequence[int],
@@ -2814,25 +3112,47 @@
         "Xavc4kProfileSettings": Xavc4kProfileSettingsTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrSettingsOutputTypeDef = TypedDict(
+    "AutomatedAbrSettingsOutputTypeDef",
+    {
+        "MaxAbrBitrate": int,
+        "MaxRenditions": int,
+        "MinAbrBitrate": int,
+        "Rules": List[AutomatedAbrRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
+CaptionDescriptionPresetOutputTypeDef = TypedDict(
+    "CaptionDescriptionPresetOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+    total=False,
+)
+
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
@@ -2863,24 +3183,50 @@
         "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
         "TrackSourceSettings": TrackSourceSettingsTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsTypeDef,
     },
     total=False,
 )
 
+RemixSettingsOutputTypeDef = TypedDict(
+    "RemixSettingsOutputTypeDef",
+    {
+        "ChannelMapping": ChannelMappingOutputTypeDef,
+        "ChannelsIn": int,
+        "ChannelsOut": int,
+    },
+    total=False,
+)
+
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
+ContainerSettingsOutputTypeDef = TypedDict(
+    "ContainerSettingsOutputTypeDef",
+    {
+        "CmfcSettings": CmfcSettingsTypeDef,
+        "Container": ContainerTypeType,
+        "F4vSettings": F4vSettingsTypeDef,
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "M3u8Settings": M3u8SettingsOutputTypeDef,
+        "MovSettings": MovSettingsTypeDef,
+        "Mp4Settings": Mp4SettingsTypeDef,
+        "MpdSettings": MpdSettingsTypeDef,
+        "MxfSettings": MxfSettingsTypeDef,
+    },
+    total=False,
+)
+
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
         "F4vSettings": F4vSettingsTypeDef,
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -2889,14 +3235,29 @@
         "Mp4Settings": Mp4SettingsTypeDef,
         "MpdSettings": MpdSettingsTypeDef,
         "MxfSettings": MxfSettingsTypeDef,
     },
     total=False,
 )
 
+VideoPreprocessorOutputTypeDef = TypedDict(
+    "VideoPreprocessorOutputTypeDef",
+    {
+        "ColorCorrector": ColorCorrectorTypeDef,
+        "Deinterlacer": DeinterlacerTypeDef,
+        "DolbyVision": DolbyVisionTypeDef,
+        "Hdr10Plus": Hdr10PlusTypeDef,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "NoiseReducer": NoiseReducerTypeDef,
+        "PartnerWatermarking": PartnerWatermarkingTypeDef,
+        "TimecodeBurnin": TimecodeBurninTypeDef,
+    },
+    total=False,
+)
+
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
         "DolbyVision": DolbyVisionTypeDef,
         "Hdr10Plus": Hdr10PlusTypeDef,
@@ -2916,40 +3277,40 @@
     total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
@@ -2972,14 +3333,22 @@
         "Vp8Settings": Vp8SettingsTypeDef,
         "Vp9Settings": Vp9SettingsTypeDef,
         "XavcSettings": XavcSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedEncodingSettingsOutputTypeDef = TypedDict(
+    "AutomatedEncodingSettingsOutputTypeDef",
+    {
+        "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
@@ -2990,14 +3359,51 @@
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
+AudioDescriptionOutputTypeDef = TypedDict(
+    "AudioDescriptionOutputTypeDef",
+    {
+        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
+        "AudioSourceName": str,
+        "AudioType": int,
+        "AudioTypeControl": AudioTypeControlType,
+        "CodecSettings": AudioCodecSettingsTypeDef,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageCodeControl": AudioLanguageCodeControlType,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "StreamName": str,
+    },
+    total=False,
+)
+
+AudioSelectorOutputTypeDef = TypedDict(
+    "AudioSelectorOutputTypeDef",
+    {
+        "AudioDurationCorrection": AudioDurationCorrectionType,
+        "CustomLanguageCode": str,
+        "DefaultSelection": AudioDefaultSelectionType,
+        "ExternalAudioFileInput": str,
+        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "Offset": int,
+        "Pids": List[int],
+        "ProgramSelection": int,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "SelectorType": AudioSelectorTypeType,
+        "Tracks": List[int],
+    },
+    total=False,
+)
+
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
@@ -3027,14 +3433,48 @@
         "RemixSettings": RemixSettingsTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": Sequence[int],
     },
     total=False,
 )
 
+CmafGroupSettingsOutputTypeDef = TypedDict(
+    "CmafGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
+        "BaseUrl": str,
+        "ClientCache": CmafClientCacheType,
+        "CodecSpecification": CmafCodecSpecificationType,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "Encryption": CmafEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsTypeDef,
+        "ManifestCompression": CmafManifestCompressionType,
+        "ManifestDurationFormat": CmafManifestDurationFormatType,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
+        "MpdProfile": CmafMpdProfileType,
+        "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
+        "SegmentControl": CmafSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": CmafSegmentLengthControlType,
+        "StreamInfResolution": CmafStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
+        "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
+        "WriteDashManifest": CmafWriteDASHManifestType,
+        "WriteHlsManifest": CmafWriteHLSManifestType,
+        "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
+    },
+    total=False,
+)
+
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
@@ -3061,14 +3501,42 @@
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
     total=False,
 )
 
+DashIsoGroupSettingsOutputTypeDef = TypedDict(
+    "DashIsoGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
+        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
+        "BaseUrl": str,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "HbbtvCompliance": DashIsoHbbtvComplianceType,
+        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsTypeDef,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
+        "MpdProfile": DashIsoMpdProfileType,
+        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
+        "SegmentControl": DashIsoSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": DashIsoSegmentLengthControlType,
+        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
+        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
+    },
+    total=False,
+)
+
 DashIsoGroupSettingsTypeDef = TypedDict(
     "DashIsoGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[DashAdditionalManifestTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
         "BaseUrl": str,
         "DashManifestStyle": DashManifestStyleType,
@@ -3098,14 +3566,53 @@
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
     },
     total=False,
 )
 
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
+        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
+        "BaseUrl": str,
+        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "Encryption": HlsEncryptionSettingsOutputTypeDef,
+        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinFinalSegmentLength": float,
+        "MinSegmentLength": int,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
+        "SegmentControl": HlsSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": HlsSegmentLengthControlType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+    },
+    total=False,
+)
+
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[HlsAdMarkersType],
         "AdditionalManifests": Sequence[HlsAdditionalManifestTypeDef],
         "AudioOnlyHeader": HlsAudioOnlyHeaderType,
         "BaseUrl": str,
@@ -3137,14 +3644,29 @@
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
     total=False,
 )
 
+MsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "MsSmoothGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
+        "AudioDeduplication": MsSmoothAudioDeduplicationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
+        "ManifestEncoding": MsSmoothManifestEncodingType,
+    },
+    total=False,
+)
+
 MsSmoothGroupSettingsTypeDef = TypedDict(
     "MsSmoothGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[MsSmoothAdditionalManifestTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
@@ -3152,14 +3674,36 @@
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
     total=False,
 )
 
+VideoDescriptionOutputTypeDef = TypedDict(
+    "VideoDescriptionOutputTypeDef",
+    {
+        "AfdSignaling": AfdSignalingType,
+        "AntiAlias": AntiAliasType,
+        "CodecSettings": VideoCodecSettingsTypeDef,
+        "ColorMetadata": ColorMetadataType,
+        "Crop": RectangleTypeDef,
+        "DropFrameTimecode": DropFrameTimecodeType,
+        "FixedAfd": int,
+        "Height": int,
+        "Position": RectangleTypeDef,
+        "RespondToAfd": RespondToAfdType,
+        "ScalingBehavior": ScalingBehaviorType,
+        "Sharpness": int,
+        "TimecodeInsertion": VideoTimecodeInsertionType,
+        "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
+        "Width": int,
+    },
+    total=False,
+)
+
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
         "CodecSettings": VideoCodecSettingsTypeDef,
         "ColorMetadata": ColorMetadataType,
@@ -3174,14 +3718,72 @@
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorTypeDef,
         "Width": int,
     },
     total=False,
 )
 
+InputOutputTypeDef = TypedDict(
+    "InputOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
+        "Crop": RectangleTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DecryptionSettings": InputDecryptionSettingsTypeDef,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FileInput": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "SupplementalImps": List[str],
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoGenerator": InputVideoGeneratorTypeDef,
+        "VideoSelector": VideoSelectorTypeDef,
+    },
+    total=False,
+)
+
+InputTemplateOutputTypeDef = TypedDict(
+    "InputTemplateOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
+        "Crop": RectangleTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoSelector": VideoSelectorTypeDef,
+    },
+    total=False,
+)
+
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
@@ -3232,27 +3834,51 @@
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorTypeDef,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
+        "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
+        "FileGroupSettings": FileGroupSettingsTypeDef,
+        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "Type": OutputGroupTypeType,
+    },
+    total=False,
+)
+
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
         "FileGroupSettings": FileGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "Type": OutputGroupTypeType,
     },
     total=False,
 )
 
+PresetSettingsOutputTypeDef = TypedDict(
+    "PresetSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "Extension": str,
@@ -3271,14 +3897,51 @@
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
+_RequiredPresetTypeDef = TypedDict(
+    "_RequiredPresetTypeDef",
+    {
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
+    },
+)
+_OptionalPresetTypeDef = TypedDict(
+    "_OptionalPresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+
+class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
+    pass
+
+
+OutputGroupOutputTypeDef = TypedDict(
+    "OutputGroupOutputTypeDef",
+    {
+        "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
+        "CustomName": str,
+        "Name": str,
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
+    },
+    total=False,
+)
+
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
@@ -3307,61 +3970,108 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
+PresetSettingsUnionTypeDef = Union[PresetSettingsTypeDef, PresetSettingsOutputTypeDef]
+_RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
-        "Settings": PresetSettingsTypeDef,
     },
 )
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
+_OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdatePresetRequestRequestTypeDef",
     {
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
+        "Settings": PresetSettingsTypeDef,
     },
     total=False,
 )
 
 
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
+class UpdatePresetRequestRequestTypeDef(
+    _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
+):
     pass
 
 
-_RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdatePresetRequestRequestTypeDef",
+CreatePresetResponseTypeDef = TypedDict(
+    "CreatePresetResponseTypeDef",
     {
-        "Name": str,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdatePresetRequestRequestTypeDef",
+
+GetPresetResponseTypeDef = TypedDict(
+    "GetPresetResponseTypeDef",
     {
-        "Category": str,
-        "Description": str,
-        "Settings": PresetSettingsTypeDef,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListPresetsResponseTypeDef = TypedDict(
+    "ListPresetsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Presets": List[PresetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdatePresetRequestRequestTypeDef(
-    _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
-):
-    pass
+UpdatePresetResponseTypeDef = TypedDict(
+    "UpdatePresetResponseTypeDef",
+    {
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+JobSettingsOutputTypeDef = TypedDict(
+    "JobSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": List[InputOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+    total=False,
+)
+
+JobTemplateSettingsOutputTypeDef = TypedDict(
+    "JobTemplateSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": List[InputTemplateOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+    total=False,
+)
 
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
         "Esam": EsamSettingsTypeDef,
@@ -3393,84 +4103,19 @@
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
     },
     total=False,
 )
 
-CreatePresetResponseTypeDef = TypedDict(
-    "CreatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPresetResponseTypeDef = TypedDict(
-    "GetPresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPresetsResponseTypeDef = TypedDict(
-    "ListPresetsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Presets": List[PresetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePresetResponseTypeDef = TypedDict(
-    "UpdatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
-        "BillingTagsSource": BillingTagsSourceType,
-        "ClientRequestToken": str,
-        "HopDestinations": Sequence[HopDestinationTypeDef],
-        "JobTemplate": str,
-        "Priority": int,
-        "Queue": str,
-        "SimulateReservedQueue": SimulateReservedQueueType,
-        "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Tags": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "Role": str,
-        "Settings": JobSettingsTypeDef,
+        "Settings": JobSettingsOutputTypeDef,
     },
 )
 _OptionalJobTypeDef = TypedDict(
     "_OptionalJobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
         "AccelerationStatus": AccelerationStatusType,
@@ -3502,73 +4147,109 @@
 )
 
 
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
 
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+_RequiredJobTemplateTypeDef = TypedDict(
+    "_RequiredJobTemplateTypeDef",
     {
         "Name": str,
-        "Settings": JobTemplateSettingsTypeDef,
+        "Settings": JobTemplateSettingsOutputTypeDef,
     },
 )
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+_OptionalJobTemplateTypeDef = TypedDict(
+    "_OptionalJobTemplateTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
+        "Arn": str,
         "Category": str,
+        "CreatedAt": datetime,
         "Description": str,
+        "HopDestinations": List[HopDestinationTypeDef],
+        "LastUpdated": datetime,
+        "Priority": int,
+        "Queue": str,
+        "StatusUpdateInterval": StatusUpdateIntervalType,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+
+class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+    pass
+
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "Role": str,
+        "Settings": JobSettingsTypeDef,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
         "HopDestinations": Sequence[HopDestinationTypeDef],
+        "JobTemplate": str,
         "Priority": int,
         "Queue": str,
+        "SimulateReservedQueue": SimulateReservedQueueType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Tags": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
+JobSettingsUnionTypeDef = Union[JobSettingsTypeDef, JobSettingsOutputTypeDef]
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
-        "LastUpdated": datetime,
+        "HopDestinations": Sequence[HopDestinationTypeDef],
         "Priority": int,
         "Queue": str,
         "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Type": TypeType,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
     pass
 
 
+JobTemplateSettingsUnionTypeDef = Union[
+    JobTemplateSettingsTypeDef, JobTemplateSettingsOutputTypeDef
+]
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJobTemplateRequestRequestTypeDef = TypedDict(
@@ -3593,60 +4274,60 @@
     pass
 
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert/type_defs.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_mediaconvert.type_defs import AacSettingsTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AacAudioDescriptionBroadcasterMixType,
     AacCodecProfileType,
     AacCodingModeType,
     AacRateControlModeType,
     AacRawFormatType,
@@ -444,14 +444,15 @@
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
     "AudioNormalizationSettingsTypeDef",
+    "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
     "Av1QvbrSettingsTypeDef",
     "AvailBlankingTypeDef",
@@ -460,46 +461,54 @@
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsTypeDef",
+    "TeletextDestinationSettingsOutputTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
+    "TeletextDestinationSettingsTypeDef",
     "CaptionSourceFramerateTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
+    "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
     "ClipLimitsTypeDef",
+    "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
-    "SpekeKeyProviderCmafTypeDef",
+    "SpekeKeyProviderCmafOutputTypeDef",
     "StaticKeyProviderTypeDef",
+    "SpekeKeyProviderCmafTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
     "CmfcSettingsTypeDef",
     "Hdr10MetadataTypeDef",
     "F4vSettingsTypeDef",
-    "M3u8SettingsTypeDef",
+    "M3u8SettingsOutputTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
+    "M3u8SettingsTypeDef",
     "HopDestinationTypeDef",
+    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
+    "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
@@ -511,149 +520,183 @@
     "GetJobTemplateRequestRequestTypeDef",
     "PolicyTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
     "H264QvbrSettingsTypeDef",
     "H265QvbrSettingsTypeDef",
     "Hdr10PlusTypeDef",
+    "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
     "HlsSettingsTypeDef",
     "Id3InsertionTypeDef",
     "InsertableImageTypeDef",
     "InputClippingTypeDef",
     "InputDecryptionSettingsTypeDef",
-    "RectangleTypeDef",
     "InputVideoGeneratorTypeDef",
+    "RectangleTypeDef",
     "JobMessagesTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
     "Mpeg2SettingsTypeDef",
+    "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
     "MxfXavcProfileSettingsTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
-    "PaginatorConfigTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationAccessControlTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "Vc3SettingsTypeDef",
     "Vp8SettingsTypeDef",
     "Vp9SettingsTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     "Xavc4kProfileSettingsTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
     "XavcHdProfileSettingsTypeDef",
     "AudioCodecSettingsTypeDef",
+    "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
     "Av1SettingsTypeDef",
     "AvcIntraSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "FileSourceSettingsTypeDef",
+    "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
+    "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    "HlsEncryptionSettingsOutputTypeDef",
+    "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DolbyVisionTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
     "H264SettingsTypeDef",
     "H265SettingsTypeDef",
     "OutputSettingsTypeDef",
+    "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
+    "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
     "MotionImageInserterTypeDef",
     "MxfSettingsTypeDef",
     "PartnerWatermarkingTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
     "QueueTypeDef",
     "S3DestinationSettingsTypeDef",
     "XavcSettingsTypeDef",
+    "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
+    "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
     "CaptionDescriptionTypeDef",
     "CaptionSourceSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
+    "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
     "DestinationSettingsTypeDef",
     "VideoCodecSettingsTypeDef",
+    "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
     "CaptionSelectorTypeDef",
+    "AudioDescriptionOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
+    "CmafGroupSettingsOutputTypeDef",
     "CmafGroupSettingsTypeDef",
+    "DashIsoGroupSettingsOutputTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
     "MsSmoothGroupSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
+    "InputOutputTypeDef",
+    "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
+    "PresetSettingsOutputTypeDef",
     "OutputTypeDef",
     "PresetSettingsTypeDef",
+    "PresetTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "PresetTypeDef",
+    "PresetSettingsUnionTypeDef",
     "UpdatePresetRequestRequestTypeDef",
-    "JobSettingsTypeDef",
-    "JobTemplateSettingsTypeDef",
     "CreatePresetResponseTypeDef",
     "GetPresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "UpdatePresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
+    "JobSettingsOutputTypeDef",
+    "JobTemplateSettingsOutputTypeDef",
+    "JobSettingsTypeDef",
+    "JobTemplateSettingsTypeDef",
     "JobTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "JobSettingsUnionTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
+    "JobTemplateSettingsUnionTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
@@ -869,14 +912,22 @@
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
     total=False,
 )
 
+AudioSelectorGroupOutputTypeDef = TypedDict(
+    "AudioSelectorGroupOutputTypeDef",
+    {
+        "AudioSelectorNames": List[str],
+    },
+    total=False,
+)
+
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
@@ -1051,19 +1102,19 @@
     "SrtDestinationSettingsTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsTypeDef = TypedDict(
-    "TeletextDestinationSettingsTypeDef",
+TeletextDestinationSettingsOutputTypeDef = TypedDict(
+    "TeletextDestinationSettingsOutputTypeDef",
     {
         "PageNumber": str,
-        "PageTypes": Sequence[TeletextPageTypeType],
+        "PageTypes": List[TeletextPageTypeType],
     },
     total=False,
 )
 
 TtmlDestinationSettingsTypeDef = TypedDict(
     "TtmlDestinationSettingsTypeDef",
     {
@@ -1077,14 +1128,23 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
+TeletextDestinationSettingsTypeDef = TypedDict(
+    "TeletextDestinationSettingsTypeDef",
+    {
+        "PageNumber": str,
+        "PageTypes": Sequence[TeletextPageTypeType],
+    },
+    total=False,
+)
+
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -1131,14 +1191,23 @@
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+OutputChannelMappingOutputTypeDef = TypedDict(
+    "OutputChannelMappingOutputTypeDef",
+    {
+        "InputChannels": List[int],
+        "InputChannelsFineTune": List[float],
+    },
+    total=False,
+)
+
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
@@ -1151,29 +1220,38 @@
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
     total=False,
 )
 
+CmafAdditionalManifestOutputTypeDef = TypedDict(
+    "CmafAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
-SpekeKeyProviderCmafTypeDef = TypedDict(
-    "SpekeKeyProviderCmafTypeDef",
+SpekeKeyProviderCmafOutputTypeDef = TypedDict(
+    "SpekeKeyProviderCmafOutputTypeDef",
     {
         "CertificateArn": str,
-        "DashSignaledSystemIds": Sequence[str],
-        "HlsSignaledSystemIds": Sequence[str],
+        "DashSignaledSystemIds": List[str],
+        "HlsSignaledSystemIds": List[str],
         "ResourceId": str,
         "Url": str,
     },
     total=False,
 )
 
 StaticKeyProviderTypeDef = TypedDict(
@@ -1183,14 +1261,26 @@
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
     total=False,
 )
 
+SpekeKeyProviderCmafTypeDef = TypedDict(
+    "SpekeKeyProviderCmafTypeDef",
+    {
+        "CertificateArn": str,
+        "DashSignaledSystemIds": Sequence[str],
+        "HlsSignaledSystemIds": Sequence[str],
+        "ResourceId": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
@@ -1244,20 +1334,20 @@
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
     total=False,
 )
 
-M3u8SettingsTypeDef = TypedDict(
-    "M3u8SettingsTypeDef",
+M3u8SettingsOutputTypeDef = TypedDict(
+    "M3u8SettingsOutputTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
-        "AudioPids": Sequence[int],
+        "AudioPids": List[int],
         "DataPTSControl": M3u8DataPtsControlType,
         "MaxPcrInterval": int,
         "NielsenId3": M3u8NielsenId3Type,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
         "PcrPid": int,
         "PmtInterval": int,
@@ -1313,42 +1403,99 @@
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
+M3u8SettingsTypeDef = TypedDict(
+    "M3u8SettingsTypeDef",
+    {
+        "AudioDuration": M3u8AudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": Sequence[int],
+        "DataPTSControl": M3u8DataPtsControlType,
+        "MaxPcrInterval": int,
+        "NielsenId3": M3u8NielsenId3Type,
+        "PatInterval": int,
+        "PcrControl": M3u8PcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "Scte35Pid": int,
+        "Scte35Source": M3u8Scte35SourceType,
+        "TimedMetadata": TimedMetadataType,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
+    },
+    total=False,
+)
+
 HopDestinationTypeDef = TypedDict(
     "HopDestinationTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
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
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
 )
 
+DashAdditionalManifestOutputTypeDef = TypedDict(
+    "DashAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "ResourceId": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+    total=False,
+)
+
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -1396,19 +1543,20 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -1571,14 +1719,23 @@
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
 )
 
+HlsAdditionalManifestOutputTypeDef = TypedDict(
+    "HlsAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -1665,33 +1822,33 @@
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
+InputVideoGeneratorTypeDef = TypedDict(
+    "InputVideoGeneratorTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
     total=False,
 )
 
-InputVideoGeneratorTypeDef = TypedDict(
-    "InputVideoGeneratorTypeDef",
-    {
-        "Duration": int,
-    },
-    total=False,
-)
-
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
     total=False,
@@ -1779,93 +1936,50 @@
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
     },
 )
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -1951,14 +2065,23 @@
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
     total=False,
 )
 
+MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
+    "MsSmoothAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+    total=False,
+)
+
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -2019,24 +2142,14 @@
     {
         "HeightInPx": int,
         "WidthInPx": int,
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
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -2062,25 +2175,14 @@
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
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
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
@@ -2257,14 +2359,26 @@
         "OpusSettings": OpusSettingsTypeDef,
         "VorbisSettings": VorbisSettingsTypeDef,
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrRuleOutputTypeDef = TypedDict(
+    "AutomatedAbrRuleOutputTypeDef",
+    {
+        "AllowedRenditions": List[AllowedRenditionSizeTypeDef],
+        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeTypeDef],
+        "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
+        "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
+        "Type": RuleTypeType,
+    },
+    total=False,
+)
+
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
@@ -2306,14 +2420,31 @@
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
     total=False,
 )
 
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
+        "DestinationType": CaptionDestinationTypeType,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
+        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
+        "ImscDestinationSettings": ImscDestinationSettingsTypeDef,
+        "SccDestinationSettings": SccDestinationSettingsTypeDef,
+        "SrtDestinationSettings": SrtDestinationSettingsTypeDef,
+        "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
+    },
+    total=False,
+)
+
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
@@ -2336,22 +2467,43 @@
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
 
+ChannelMappingOutputTypeDef = TypedDict(
+    "ChannelMappingOutputTypeDef",
+    {
+        "OutputChannels": List[OutputChannelMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
     total=False,
 )
 
+CmafEncryptionSettingsOutputTypeDef = TypedDict(
+    "CmafEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": CmafEncryptionTypeType,
+        "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
+        "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "Type": CmafKeyProviderTypeType,
+    },
+    total=False,
+)
+
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
@@ -2435,14 +2587,45 @@
 )
 
 class UpdateQueueRequestRequestTypeDef(
     _RequiredUpdateQueueRequestRequestTypeDef, _OptionalUpdateQueueRequestRequestTypeDef
 ):
     pass
 
+DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    {
+        "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+    total=False,
+)
+
+HlsEncryptionSettingsOutputTypeDef = TypedDict(
+    "HlsEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": HlsEncryptionTypeType,
+        "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
+        "OfflineEncrypted": HlsOfflineEncryptedType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "Type": HlsKeyProviderTypeType,
+    },
+    total=False,
+)
+
+MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
+    "MsSmoothEncryptionSettingsOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+    total=False,
+)
+
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
@@ -2466,20 +2649,72 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    {
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
@@ -2500,30 +2735,30 @@
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPolicyRequestRequestTypeDef = TypedDict(
     "PutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2625,37 +2860,100 @@
     "OutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
     },
     total=False,
 )
 
+TimedMetadataInsertionOutputTypeDef = TypedDict(
+    "TimedMetadataInsertionOutputTypeDef",
+    {
+        "Id3Insertions": List[Id3InsertionTypeDef],
+    },
+    total=False,
+)
+
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
+ImageInserterOutputTypeDef = TypedDict(
+    "ImageInserterOutputTypeDef",
+    {
+        "InsertableImages": List[InsertableImageTypeDef],
+        "SdrReferenceWhiteLevel": int,
+    },
+    total=False,
+)
+
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+M2tsSettingsOutputTypeDef = TypedDict(
+    "M2tsSettingsOutputTypeDef",
+    {
+        "AudioBufferModel": M2tsAudioBufferModelType,
+        "AudioDuration": M2tsAudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": List[int],
+        "Bitrate": int,
+        "BufferModel": M2tsBufferModelType,
+        "DataPTSControl": M2tsDataPtsControlType,
+        "DvbNitSettings": DvbNitSettingsTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsTypeDef,
+        "DvbSubPids": List[int],
+        "DvbTdtSettings": DvbTdtSettingsTypeDef,
+        "DvbTeletextPid": int,
+        "EbpAudioInterval": M2tsEbpAudioIntervalType,
+        "EbpPlacement": M2tsEbpPlacementType,
+        "EsRateInPes": M2tsEsRateInPesType,
+        "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
+        "FragmentTime": float,
+        "KlvMetadata": M2tsKlvMetadataType,
+        "MaxPcrInterval": int,
+        "MinEbpInterval": int,
+        "NielsenId3": M2tsNielsenId3Type,
+        "NullPacketBitrate": float,
+        "PatInterval": int,
+        "PcrControl": M2tsPcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "RateMode": M2tsRateModeType,
+        "Scte35Esam": M2tsScte35EsamTypeDef,
+        "Scte35Pid": int,
+        "Scte35Source": M2tsScte35SourceType,
+        "SegmentationMarkers": M2tsSegmentationMarkersType,
+        "SegmentationStyle": M2tsSegmentationStyleType,
+        "SegmentationTime": float,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
     },
+    total=False,
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
@@ -2805,25 +3103,47 @@
         "Xavc4kProfileSettings": Xavc4kProfileSettingsTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrSettingsOutputTypeDef = TypedDict(
+    "AutomatedAbrSettingsOutputTypeDef",
+    {
+        "MaxAbrBitrate": int,
+        "MaxRenditions": int,
+        "MinAbrBitrate": int,
+        "Rules": List[AutomatedAbrRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
+CaptionDescriptionPresetOutputTypeDef = TypedDict(
+    "CaptionDescriptionPresetOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+    total=False,
+)
+
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
@@ -2854,24 +3174,50 @@
         "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
         "TrackSourceSettings": TrackSourceSettingsTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsTypeDef,
     },
     total=False,
 )
 
+RemixSettingsOutputTypeDef = TypedDict(
+    "RemixSettingsOutputTypeDef",
+    {
+        "ChannelMapping": ChannelMappingOutputTypeDef,
+        "ChannelsIn": int,
+        "ChannelsOut": int,
+    },
+    total=False,
+)
+
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
+ContainerSettingsOutputTypeDef = TypedDict(
+    "ContainerSettingsOutputTypeDef",
+    {
+        "CmfcSettings": CmfcSettingsTypeDef,
+        "Container": ContainerTypeType,
+        "F4vSettings": F4vSettingsTypeDef,
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "M3u8Settings": M3u8SettingsOutputTypeDef,
+        "MovSettings": MovSettingsTypeDef,
+        "Mp4Settings": Mp4SettingsTypeDef,
+        "MpdSettings": MpdSettingsTypeDef,
+        "MxfSettings": MxfSettingsTypeDef,
+    },
+    total=False,
+)
+
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
         "F4vSettings": F4vSettingsTypeDef,
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -2880,14 +3226,29 @@
         "Mp4Settings": Mp4SettingsTypeDef,
         "MpdSettings": MpdSettingsTypeDef,
         "MxfSettings": MxfSettingsTypeDef,
     },
     total=False,
 )
 
+VideoPreprocessorOutputTypeDef = TypedDict(
+    "VideoPreprocessorOutputTypeDef",
+    {
+        "ColorCorrector": ColorCorrectorTypeDef,
+        "Deinterlacer": DeinterlacerTypeDef,
+        "DolbyVision": DolbyVisionTypeDef,
+        "Hdr10Plus": Hdr10PlusTypeDef,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "NoiseReducer": NoiseReducerTypeDef,
+        "PartnerWatermarking": PartnerWatermarkingTypeDef,
+        "TimecodeBurnin": TimecodeBurninTypeDef,
+    },
+    total=False,
+)
+
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
         "DolbyVision": DolbyVisionTypeDef,
         "Hdr10Plus": Hdr10PlusTypeDef,
@@ -2907,40 +3268,40 @@
     total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
@@ -2963,14 +3324,22 @@
         "Vp8Settings": Vp8SettingsTypeDef,
         "Vp9Settings": Vp9SettingsTypeDef,
         "XavcSettings": XavcSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedEncodingSettingsOutputTypeDef = TypedDict(
+    "AutomatedEncodingSettingsOutputTypeDef",
+    {
+        "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
@@ -2981,14 +3350,51 @@
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
+AudioDescriptionOutputTypeDef = TypedDict(
+    "AudioDescriptionOutputTypeDef",
+    {
+        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
+        "AudioSourceName": str,
+        "AudioType": int,
+        "AudioTypeControl": AudioTypeControlType,
+        "CodecSettings": AudioCodecSettingsTypeDef,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageCodeControl": AudioLanguageCodeControlType,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "StreamName": str,
+    },
+    total=False,
+)
+
+AudioSelectorOutputTypeDef = TypedDict(
+    "AudioSelectorOutputTypeDef",
+    {
+        "AudioDurationCorrection": AudioDurationCorrectionType,
+        "CustomLanguageCode": str,
+        "DefaultSelection": AudioDefaultSelectionType,
+        "ExternalAudioFileInput": str,
+        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "Offset": int,
+        "Pids": List[int],
+        "ProgramSelection": int,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "SelectorType": AudioSelectorTypeType,
+        "Tracks": List[int],
+    },
+    total=False,
+)
+
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
@@ -3018,14 +3424,48 @@
         "RemixSettings": RemixSettingsTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": Sequence[int],
     },
     total=False,
 )
 
+CmafGroupSettingsOutputTypeDef = TypedDict(
+    "CmafGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
+        "BaseUrl": str,
+        "ClientCache": CmafClientCacheType,
+        "CodecSpecification": CmafCodecSpecificationType,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "Encryption": CmafEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsTypeDef,
+        "ManifestCompression": CmafManifestCompressionType,
+        "ManifestDurationFormat": CmafManifestDurationFormatType,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
+        "MpdProfile": CmafMpdProfileType,
+        "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
+        "SegmentControl": CmafSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": CmafSegmentLengthControlType,
+        "StreamInfResolution": CmafStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
+        "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
+        "WriteDashManifest": CmafWriteDASHManifestType,
+        "WriteHlsManifest": CmafWriteHLSManifestType,
+        "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
+    },
+    total=False,
+)
+
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
@@ -3052,14 +3492,42 @@
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
     total=False,
 )
 
+DashIsoGroupSettingsOutputTypeDef = TypedDict(
+    "DashIsoGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
+        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
+        "BaseUrl": str,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "HbbtvCompliance": DashIsoHbbtvComplianceType,
+        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsTypeDef,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
+        "MpdProfile": DashIsoMpdProfileType,
+        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
+        "SegmentControl": DashIsoSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": DashIsoSegmentLengthControlType,
+        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
+        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
+    },
+    total=False,
+)
+
 DashIsoGroupSettingsTypeDef = TypedDict(
     "DashIsoGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[DashAdditionalManifestTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
         "BaseUrl": str,
         "DashManifestStyle": DashManifestStyleType,
@@ -3089,14 +3557,53 @@
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
     },
     total=False,
 )
 
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
+        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
+        "BaseUrl": str,
+        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "Encryption": HlsEncryptionSettingsOutputTypeDef,
+        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinFinalSegmentLength": float,
+        "MinSegmentLength": int,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
+        "SegmentControl": HlsSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": HlsSegmentLengthControlType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+    },
+    total=False,
+)
+
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[HlsAdMarkersType],
         "AdditionalManifests": Sequence[HlsAdditionalManifestTypeDef],
         "AudioOnlyHeader": HlsAudioOnlyHeaderType,
         "BaseUrl": str,
@@ -3128,14 +3635,29 @@
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
     total=False,
 )
 
+MsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "MsSmoothGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
+        "AudioDeduplication": MsSmoothAudioDeduplicationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsTypeDef,
+        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
+        "ManifestEncoding": MsSmoothManifestEncodingType,
+    },
+    total=False,
+)
+
 MsSmoothGroupSettingsTypeDef = TypedDict(
     "MsSmoothGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[MsSmoothAdditionalManifestTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
@@ -3143,14 +3665,36 @@
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
     total=False,
 )
 
+VideoDescriptionOutputTypeDef = TypedDict(
+    "VideoDescriptionOutputTypeDef",
+    {
+        "AfdSignaling": AfdSignalingType,
+        "AntiAlias": AntiAliasType,
+        "CodecSettings": VideoCodecSettingsTypeDef,
+        "ColorMetadata": ColorMetadataType,
+        "Crop": RectangleTypeDef,
+        "DropFrameTimecode": DropFrameTimecodeType,
+        "FixedAfd": int,
+        "Height": int,
+        "Position": RectangleTypeDef,
+        "RespondToAfd": RespondToAfdType,
+        "ScalingBehavior": ScalingBehaviorType,
+        "Sharpness": int,
+        "TimecodeInsertion": VideoTimecodeInsertionType,
+        "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
+        "Width": int,
+    },
+    total=False,
+)
+
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
         "CodecSettings": VideoCodecSettingsTypeDef,
         "ColorMetadata": ColorMetadataType,
@@ -3165,14 +3709,72 @@
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorTypeDef,
         "Width": int,
     },
     total=False,
 )
 
+InputOutputTypeDef = TypedDict(
+    "InputOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
+        "Crop": RectangleTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DecryptionSettings": InputDecryptionSettingsTypeDef,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FileInput": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "SupplementalImps": List[str],
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoGenerator": InputVideoGeneratorTypeDef,
+        "VideoSelector": VideoSelectorTypeDef,
+    },
+    total=False,
+)
+
+InputTemplateOutputTypeDef = TypedDict(
+    "InputTemplateOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
+        "Crop": RectangleTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoSelector": VideoSelectorTypeDef,
+    },
+    total=False,
+)
+
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
@@ -3223,27 +3825,51 @@
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorTypeDef,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
+        "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
+        "FileGroupSettings": FileGroupSettingsTypeDef,
+        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "Type": OutputGroupTypeType,
+    },
+    total=False,
+)
+
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
         "FileGroupSettings": FileGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "Type": OutputGroupTypeType,
     },
     total=False,
 )
 
+PresetSettingsOutputTypeDef = TypedDict(
+    "PresetSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "Extension": str,
@@ -3262,14 +3888,49 @@
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
+_RequiredPresetTypeDef = TypedDict(
+    "_RequiredPresetTypeDef",
+    {
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
+    },
+)
+_OptionalPresetTypeDef = TypedDict(
+    "_OptionalPresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
+    pass
+
+OutputGroupOutputTypeDef = TypedDict(
+    "OutputGroupOutputTypeDef",
+    {
+        "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
+        "CustomName": str,
+        "Name": str,
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
+    },
+    total=False,
+)
+
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
@@ -3296,57 +3957,106 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
+PresetSettingsUnionTypeDef = Union[PresetSettingsTypeDef, PresetSettingsOutputTypeDef]
+_RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
-        "Settings": PresetSettingsTypeDef,
     },
 )
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
+_OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdatePresetRequestRequestTypeDef",
     {
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
+        "Settings": PresetSettingsTypeDef,
     },
     total=False,
 )
 
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
+class UpdatePresetRequestRequestTypeDef(
+    _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
+):
     pass
 
-_RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdatePresetRequestRequestTypeDef",
+CreatePresetResponseTypeDef = TypedDict(
+    "CreatePresetResponseTypeDef",
     {
-        "Name": str,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdatePresetRequestRequestTypeDef",
+
+GetPresetResponseTypeDef = TypedDict(
+    "GetPresetResponseTypeDef",
     {
-        "Category": str,
-        "Description": str,
-        "Settings": PresetSettingsTypeDef,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPresetsResponseTypeDef = TypedDict(
+    "ListPresetsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Presets": List[PresetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePresetResponseTypeDef = TypedDict(
+    "UpdatePresetResponseTypeDef",
+    {
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobSettingsOutputTypeDef = TypedDict(
+    "JobSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": List[InputOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
     total=False,
 )
 
-class UpdatePresetRequestRequestTypeDef(
-    _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
-):
-    pass
+JobTemplateSettingsOutputTypeDef = TypedDict(
+    "JobTemplateSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": List[InputTemplateOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+    total=False,
+)
 
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
         "Esam": EsamSettingsTypeDef,
@@ -3378,82 +4088,19 @@
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
     },
     total=False,
 )
 
-CreatePresetResponseTypeDef = TypedDict(
-    "CreatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPresetResponseTypeDef = TypedDict(
-    "GetPresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPresetsResponseTypeDef = TypedDict(
-    "ListPresetsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Presets": List[PresetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePresetResponseTypeDef = TypedDict(
-    "UpdatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
-        "BillingTagsSource": BillingTagsSourceType,
-        "ClientRequestToken": str,
-        "HopDestinations": Sequence[HopDestinationTypeDef],
-        "JobTemplate": str,
-        "Priority": int,
-        "Queue": str,
-        "SimulateReservedQueue": SimulateReservedQueueType,
-        "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Tags": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "Role": str,
-        "Settings": JobSettingsTypeDef,
+        "Settings": JobSettingsOutputTypeDef,
     },
 )
 _OptionalJobTypeDef = TypedDict(
     "_OptionalJobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
         "AccelerationStatus": AccelerationStatusType,
@@ -3483,69 +4130,103 @@
     },
     total=False,
 )
 
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+_RequiredJobTemplateTypeDef = TypedDict(
+    "_RequiredJobTemplateTypeDef",
     {
         "Name": str,
-        "Settings": JobTemplateSettingsTypeDef,
+        "Settings": JobTemplateSettingsOutputTypeDef,
     },
 )
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+_OptionalJobTemplateTypeDef = TypedDict(
+    "_OptionalJobTemplateTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
+        "Arn": str,
         "Category": str,
+        "CreatedAt": datetime,
         "Description": str,
+        "HopDestinations": List[HopDestinationTypeDef],
+        "LastUpdated": datetime,
+        "Priority": int,
+        "Queue": str,
+        "StatusUpdateInterval": StatusUpdateIntervalType,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+    pass
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "Role": str,
+        "Settings": JobSettingsTypeDef,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
         "HopDestinations": Sequence[HopDestinationTypeDef],
+        "JobTemplate": str,
         "Priority": int,
         "Queue": str,
+        "SimulateReservedQueue": SimulateReservedQueueType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Tags": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
+JobSettingsUnionTypeDef = Union[JobSettingsTypeDef, JobSettingsOutputTypeDef]
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
-        "LastUpdated": datetime,
+        "HopDestinations": Sequence[HopDestinationTypeDef],
         "Priority": int,
         "Queue": str,
         "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Type": TypeType,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
     pass
 
+JobTemplateSettingsUnionTypeDef = Union[
+    JobTemplateSettingsTypeDef, JobTemplateSettingsOutputTypeDef
+]
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJobTemplateRequestRequestTypeDef = TypedDict(
@@ -3568,60 +4249,60 @@
 ):
     pass
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/PKG-INFO` & `types-aiobotocore-mediaconvert-2.5.2.post1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-mediaconvert
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mediaconvert"></a>
 
 # types-aiobotocore-mediaconvert
 
 [![PyPI - types-aiobotocore-mediaconvert](https://img.shields.io/pypi/v/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mediaconvert?color=blue)](https://pypistats.org/packages/types-aiobotocore-mediaconvert)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MediaConvert 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [types-aiobotocore-mediaconvert docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/).
 
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
@@ -731,20 +698,20 @@
 )
 
 
 def check_value(value: AacAudioDescriptionBroadcasterMixType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mediaconvert.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mediaconvert.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AccelerationSettingsTypeDef,
     AdvancedInputFilterSettingsTypeDef,
@@ -757,14 +724,15 @@
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
     HlsRenditionGroupSettingsTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
     Av1QvbrSettingsTypeDef,
     AvailBlankingTypeDef,
@@ -773,46 +741,54 @@
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
-    TeletextDestinationSettingsTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    TeletextDestinationSettingsTypeDef,
     CaptionSourceFramerateTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
+    OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
     ClipLimitsTypeDef,
+    CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
-    SpekeKeyProviderCmafTypeDef,
+    SpekeKeyProviderCmafOutputTypeDef,
     StaticKeyProviderTypeDef,
+    SpekeKeyProviderCmafTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
     CmfcSettingsTypeDef,
     Hdr10MetadataTypeDef,
     F4vSettingsTypeDef,
-    M3u8SettingsTypeDef,
+    M3u8SettingsOutputTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
+    M3u8SettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
+    DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
@@ -824,161 +800,195 @@
     GetJobTemplateRequestRequestTypeDef,
     PolicyTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
     H264QvbrSettingsTypeDef,
     H265QvbrSettingsTypeDef,
     Hdr10PlusTypeDef,
+    HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
     HlsCaptionLanguageMappingTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
     HlsSettingsTypeDef,
     Id3InsertionTypeDef,
     InsertableImageTypeDef,
     InputClippingTypeDef,
     InputDecryptionSettingsTypeDef,
-    RectangleTypeDef,
     InputVideoGeneratorTypeDef,
+    RectangleTypeDef,
     JobMessagesTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
     Mpeg2SettingsTypeDef,
+    MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
     MxfXavcProfileSettingsTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
     Vc3SettingsTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
     Xavc4kProfileSettingsTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
     XavcHdProfileSettingsTypeDef,
     AudioCodecSettingsTypeDef,
+    AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
     Av1SettingsTypeDef,
     AvcIntraSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
     FileSourceSettingsTypeDef,
+    ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
+    CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
+    DashIsoEncryptionSettingsOutputTypeDef,
+    HlsEncryptionSettingsOutputTypeDef,
+    MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
     H264SettingsTypeDef,
     H265SettingsTypeDef,
     OutputSettingsTypeDef,
+    TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
+    ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
+    M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
     MotionImageInserterTypeDef,
     MxfSettingsTypeDef,
     PartnerWatermarkingTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
     QueueTypeDef,
     S3DestinationSettingsTypeDef,
     XavcSettingsTypeDef,
+    AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
     CaptionDescriptionTypeDef,
     CaptionSourceSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
+    VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
     DestinationSettingsTypeDef,
     VideoCodecSettingsTypeDef,
+    AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
     CaptionSelectorTypeDef,
+    AudioDescriptionOutputTypeDef,
+    AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
+    CmafGroupSettingsOutputTypeDef,
     CmafGroupSettingsTypeDef,
+    DashIsoGroupSettingsOutputTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
+    HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
+    InputOutputTypeDef,
+    InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
+    PresetSettingsOutputTypeDef,
     OutputTypeDef,
     PresetSettingsTypeDef,
+    PresetTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
     CreatePresetRequestRequestTypeDef,
-    PresetTypeDef,
+    PresetSettingsUnionTypeDef,
     UpdatePresetRequestRequestTypeDef,
-    JobSettingsTypeDef,
-    JobTemplateSettingsTypeDef,
     CreatePresetResponseTypeDef,
     GetPresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     UpdatePresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
+    JobSettingsOutputTypeDef,
+    JobTemplateSettingsOutputTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     JobTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobRequestRequestTypeDef,
+    JobSettingsUnionTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
+    JobTemplateSettingsUnionTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_value() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*


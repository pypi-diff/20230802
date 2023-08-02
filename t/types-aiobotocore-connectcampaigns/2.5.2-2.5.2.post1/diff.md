# Comparing `tmp/types-aiobotocore-connectcampaigns-2.5.2.tar.gz` & `tmp/types-aiobotocore-connectcampaigns-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.tar", last modified: Sat Jul  8 01:43:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
```

## Comparing `types-aiobotocore-connectcampaigns-2.5.2.tar` & `types-aiobotocore-connectcampaigns-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.249953 types-aiobotocore-connectcampaigns-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-08 01:43:28.249953 types-aiobotocore-connectcampaigns-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:28.249953 types-aiobotocore-connectcampaigns-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-08 01:28:15.000000 types-aiobotocore-connectcampaigns-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.241953 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:16.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.249953 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-08 01:43:28.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:43:28.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:28.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:28.000000 types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.237613 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/LICENSE` & `types-aiobotocore-connectcampaigns-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore connectcampaigns type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectcampaigns"></a>
 
 # types-aiobotocore-connectcampaigns
 
 [![PyPI - types-aiobotocore-connectcampaigns](https://img.shields.io/pypi/v/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectcampaigns?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectcampaigns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcampaigns)](https://pepy.tech/project/types-aiobotocore-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectCampaignService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [types-aiobotocore-connectcampaigns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/).
 
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
@@ -312,80 +311,81 @@
 )
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectcampaigns.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    CreateCampaignResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
-    DialRequestTypeDef,
+    TimestampTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
-    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
+    CreateCampaignResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    DialRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    PutDialRequestBatchRequestRequestTypeDef,
     CampaignTypeDef,
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/README.md` & `types-aiobotocore-connectcampaigns-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-connectcampaigns"></a>
 
 # types-aiobotocore-connectcampaigns
 
 [![PyPI - types-aiobotocore-connectcampaigns](https://img.shields.io/pypi/v/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectcampaigns?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectcampaigns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcampaigns)](https://pepy.tech/project/types-aiobotocore-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectCampaignService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [types-aiobotocore-connectcampaigns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/).
 
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
@@ -279,80 +279,81 @@
 )
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectcampaigns.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    CreateCampaignResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
-    DialRequestTypeDef,
+    TimestampTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
-    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
+    CreateCampaignResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    DialRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    PutDialRequestBatchRequestRequestTypeDef,
     CampaignTypeDef,
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/setup.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcampaigns",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with"
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
-    keywords="aiobotocore connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore connectcampaigns type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_connectcampaigns": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/"
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/__init__.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/__init__.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/__main__.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConnectCampaignService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/client.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/client.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/literals.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/literals.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/paginator.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,34 +25,31 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import CampaignFiltersTypeDef, ListCampaignsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListCampaignsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListCampaignsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: CampaignFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/paginators/#listcampaignspaginator)
         """
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/paginator.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,34 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import CampaignFiltersTypeDef, ListCampaignsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListCampaignsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListCampaignsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: CampaignFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/paginators/#listcampaignspaginator)
         """
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/type_defs.py` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
-    data: AnswerMachineDetectionConfigTypeDef = {...}
+    data: AnswerMachineDetectionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,59 +33,60 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
-    "CreateCampaignResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
-    "DialRequestTypeDef",
+    "TimestampTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
-    "GetCampaignStateResponseTypeDef",
     "GetConnectInstanceConfigRequestRequestTypeDef",
     "GetInstanceOnboardingJobStatusRequestRequestTypeDef",
     "InstanceOnboardingJobStatusTypeDef",
-    "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "PauseCampaignRequestRequestTypeDef",
     "SuccessfulRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
-    "PutDialRequestBatchRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "DialRequestTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "PutDialRequestBatchRequestRequestTypeDef",
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
@@ -110,21 +111,22 @@
         "arn": str,
         "connectInstanceId": str,
         "id": str,
         "name": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
@@ -148,45 +150,29 @@
 DescribeCampaignRequestRequestTypeDef = TypedDict(
     "DescribeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DialRequestTypeDef = TypedDict(
-    "DialRequestTypeDef",
-    {
-        "attributes": Mapping[str, str],
-        "clientToken": str,
-        "expirationTime": Union[datetime, str],
-        "phoneNumber": str,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
 ProgressiveDialerConfigTypeDef = TypedDict(
     "ProgressiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -241,22 +227,14 @@
 GetCampaignStateRequestRequestTypeDef = TypedDict(
     "GetCampaignStateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetCampaignStateResponseTypeDef = TypedDict(
-    "GetCampaignStateResponseTypeDef",
-    {
-        "state": CampaignStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConnectInstanceConfigRequestRequestTypeDef = TypedDict(
     "GetConnectInstanceConfigRequestRequestTypeDef",
     {
         "connectInstanceId": str,
     },
 )
 
@@ -285,39 +263,31 @@
 
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 PauseCampaignRequestRequestTypeDef = TypedDict(
     "PauseCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -326,25 +296,14 @@
     {
         "clientToken": str,
         "id": str,
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
 ResumeCampaignRequestRequestTypeDef = TypedDict(
     "ResumeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -437,28 +396,63 @@
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
 
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
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
+GetCampaignStateResponseTypeDef = TypedDict(
+    "GetCampaignStateResponseTypeDef",
+    {
+        "state": CampaignStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaryList": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutDialRequestBatchRequestRequestTypeDef = TypedDict(
-    "PutDialRequestBatchRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "dialRequests": Sequence[DialRequestTypeDef],
-        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DialRequestTypeDef = TypedDict(
+    "DialRequestTypeDef",
+    {
+        "attributes": Mapping[str, str],
+        "clientToken": str,
+        "expirationTime": TimestampTypeDef,
+        "phoneNumber": str,
     },
 )
 
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
@@ -485,62 +479,70 @@
 )
 
 GetCampaignStateBatchResponseTypeDef = TypedDict(
     "GetCampaignStateBatchResponseTypeDef",
     {
         "failedRequests": List[FailedCampaignStateResponseTypeDef],
         "successfulRequests": List[SuccessfulCampaignStateResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceOnboardingJobStatusResponseTypeDef = TypedDict(
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartInstanceOnboardingJobResponseTypeDef = TypedDict(
     "StartInstanceOnboardingJobResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDialRequestBatchResponseTypeDef = TypedDict(
     "PutDialRequestBatchResponseTypeDef",
     {
         "failedRequests": List[FailedRequestTypeDef],
         "successfulRequests": List[SuccessfulRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+PutDialRequestBatchRequestRequestTypeDef = TypedDict(
+    "PutDialRequestBatchRequestRequestTypeDef",
+    {
+        "dialRequests": Sequence[DialRequestTypeDef],
+        "id": str,
+    },
+)
+
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
         "dialerConfig": DialerConfigTypeDef,
         "id": str,
@@ -593,18 +595,18 @@
     },
 )
 
 GetConnectInstanceConfigResponseTypeDef = TypedDict(
     "GetConnectInstanceConfigResponseTypeDef",
     {
         "connectInstanceConfig": InstanceConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCampaignResponseTypeDef = TypedDict(
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns/type_defs.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
-    data: AnswerMachineDetectionConfigTypeDef = {...}
+    data: AnswerMachineDetectionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -32,59 +32,60 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
-    "CreateCampaignResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
-    "DialRequestTypeDef",
+    "TimestampTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
-    "GetCampaignStateResponseTypeDef",
     "GetConnectInstanceConfigRequestRequestTypeDef",
     "GetInstanceOnboardingJobStatusRequestRequestTypeDef",
     "InstanceOnboardingJobStatusTypeDef",
-    "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "PauseCampaignRequestRequestTypeDef",
     "SuccessfulRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
-    "PutDialRequestBatchRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "DialRequestTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "PutDialRequestBatchRequestRequestTypeDef",
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
@@ -109,21 +110,22 @@
         "arn": str,
         "connectInstanceId": str,
         "id": str,
         "name": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
@@ -147,45 +149,29 @@
 DescribeCampaignRequestRequestTypeDef = TypedDict(
     "DescribeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DialRequestTypeDef = TypedDict(
-    "DialRequestTypeDef",
-    {
-        "attributes": Mapping[str, str],
-        "clientToken": str,
-        "expirationTime": Union[datetime, str],
-        "phoneNumber": str,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
 ProgressiveDialerConfigTypeDef = TypedDict(
     "ProgressiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -238,22 +224,14 @@
 GetCampaignStateRequestRequestTypeDef = TypedDict(
     "GetCampaignStateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetCampaignStateResponseTypeDef = TypedDict(
-    "GetCampaignStateResponseTypeDef",
-    {
-        "state": CampaignStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConnectInstanceConfigRequestRequestTypeDef = TypedDict(
     "GetConnectInstanceConfigRequestRequestTypeDef",
     {
         "connectInstanceId": str,
     },
 )
 
@@ -280,39 +258,31 @@
 )
 
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 PauseCampaignRequestRequestTypeDef = TypedDict(
     "PauseCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -321,25 +291,14 @@
     {
         "clientToken": str,
         "id": str,
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
 ResumeCampaignRequestRequestTypeDef = TypedDict(
     "ResumeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -428,28 +387,63 @@
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
 
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
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
+GetCampaignStateResponseTypeDef = TypedDict(
+    "GetCampaignStateResponseTypeDef",
+    {
+        "state": CampaignStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaryList": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutDialRequestBatchRequestRequestTypeDef = TypedDict(
-    "PutDialRequestBatchRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "dialRequests": Sequence[DialRequestTypeDef],
-        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DialRequestTypeDef = TypedDict(
+    "DialRequestTypeDef",
+    {
+        "attributes": Mapping[str, str],
+        "clientToken": str,
+        "expirationTime": TimestampTypeDef,
+        "phoneNumber": str,
     },
 )
 
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
@@ -476,62 +470,70 @@
 )
 
 GetCampaignStateBatchResponseTypeDef = TypedDict(
     "GetCampaignStateBatchResponseTypeDef",
     {
         "failedRequests": List[FailedCampaignStateResponseTypeDef],
         "successfulRequests": List[SuccessfulCampaignStateResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceOnboardingJobStatusResponseTypeDef = TypedDict(
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartInstanceOnboardingJobResponseTypeDef = TypedDict(
     "StartInstanceOnboardingJobResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDialRequestBatchResponseTypeDef = TypedDict(
     "PutDialRequestBatchResponseTypeDef",
     {
         "failedRequests": List[FailedRequestTypeDef],
         "successfulRequests": List[SuccessfulRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+PutDialRequestBatchRequestRequestTypeDef = TypedDict(
+    "PutDialRequestBatchRequestRequestTypeDef",
+    {
+        "dialRequests": Sequence[DialRequestTypeDef],
+        "id": str,
+    },
+)
+
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
         "dialerConfig": DialerConfigTypeDef,
         "id": str,
@@ -580,18 +582,18 @@
     },
 )
 
 GetConnectInstanceConfigResponseTypeDef = TypedDict(
     "GetConnectInstanceConfigResponseTypeDef",
     {
         "connectInstanceConfig": InstanceConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCampaignResponseTypeDef = TypedDict(
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore connectcampaigns type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectcampaigns"></a>
 
 # types-aiobotocore-connectcampaigns
 
 [![PyPI - types-aiobotocore-connectcampaigns](https://img.shields.io/pypi/v/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectcampaigns?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectcampaigns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcampaigns)](https://pepy.tech/project/types-aiobotocore-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectCampaignService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [types-aiobotocore-connectcampaigns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/).
 
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
@@ -312,80 +311,81 @@
 )
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectcampaigns.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    CreateCampaignResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
-    DialRequestTypeDef,
+    TimestampTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
-    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
+    CreateCampaignResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    DialRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    PutDialRequestBatchRequestRequestTypeDef,
     CampaignTypeDef,
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt` & `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*


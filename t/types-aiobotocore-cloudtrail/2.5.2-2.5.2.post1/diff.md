# Comparing `tmp/types-aiobotocore-cloudtrail-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudtrail-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudtrail-2.5.2.tar", last modified: Sat Jul  8 01:43:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudtrail-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-cloudtrail-2.5.2.tar` & `types-aiobotocore-cloudtrail-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:22.821849 types-aiobotocore-cloudtrail-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-07-08 01:43:22.821849 types-aiobotocore-cloudtrail-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:22.821849 types-aiobotocore-cloudtrail-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:22.821849 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41336 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41275 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39834 2023-07-08 01:27:14.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39799 2023-07-08 01:27:13.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:12.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:22.821849 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.253627 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41873 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/LICENSE` & `types-aiobotocore-cloudtrail-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2/PKG-INFO` & `types-aiobotocore-cloudtrail-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudtrail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudtrail type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudtrail"></a>
 
 # types-aiobotocore-cloudtrail
 
 [![PyPI - types-aiobotocore-cloudtrail](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudtrail?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudtrail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudTrail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [types-aiobotocore-cloudtrail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/).
 
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
@@ -334,30 +333,31 @@
 )
 
 
 def check_value(value: DeliveryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudtrail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudtrail.type_defs import (
     TagTypeDef,
+    AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
-    CreateTrailResponseTypeDef,
+    DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -372,103 +372,109 @@
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
     InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
-    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
-    ListPublicKeysRequestRequestTypeDef,
+    TimestampTypeDef,
     PublicKeyTypeDef,
-    ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
     StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
-    StartQueryResponseTypeDef,
     StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
-    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     ResourceTagTypeDef,
+    AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateTrailResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetTrailStatusResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartQueryResponseTypeDef,
+    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
     PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListPublicKeysRequestRequestTypeDef,
+    ListQueriesRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreResponseTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     GetEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
     PutEventSelectorsResponseTypeDef,
+    EventSelectorUnionTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/README.md` & `types-aiobotocore-cloudtrail-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudtrail"></a>
 
 # types-aiobotocore-cloudtrail
 
 [![PyPI - types-aiobotocore-cloudtrail](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudtrail?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudtrail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudTrail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [types-aiobotocore-cloudtrail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/).
 
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
@@ -301,30 +301,31 @@
 )
 
 
 def check_value(value: DeliveryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudtrail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudtrail.type_defs import (
     TagTypeDef,
+    AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
-    CreateTrailResponseTypeDef,
+    DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -339,103 +340,109 @@
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
     InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
-    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
-    ListPublicKeysRequestRequestTypeDef,
+    TimestampTypeDef,
     PublicKeyTypeDef,
-    ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
     StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
-    StartQueryResponseTypeDef,
     StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
-    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     ResourceTagTypeDef,
+    AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateTrailResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetTrailStatusResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartQueryResponseTypeDef,
+    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
     PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListPublicKeysRequestRequestTypeDef,
+    ListQueriesRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreResponseTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     GetEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
     PutEventSelectorsResponseTypeDef,
+    EventSelectorUnionTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/setup.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudtrail",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudtrail type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudtrail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudtrail": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/"
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/__init__.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/__init__.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/__main__.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudTrail 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudTrail 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
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

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/client.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,39 +11,38 @@
 
     session = get_session()
     async with session.create_client("cloudtrail") as client:
         client: CloudTrailClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ImportStatusType, QueryStatusType
 from .paginator import (
     ListImportFailuresPaginator,
     ListImportsPaginator,
     ListPublicKeysPaginator,
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 from .type_defs import (
-    AdvancedEventSelectorTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     CancelQueryResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     CreateTrailResponseTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     DestinationTypeDef,
-    EventSelectorTypeDef,
+    EventSelectorUnionTypeDef,
     GetChannelResponseTypeDef,
     GetEventDataStoreResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     GetImportResponseTypeDef,
     GetInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
@@ -65,14 +64,15 @@
     PutInsightSelectorsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     StartImportResponseTypeDef,
     StartQueryResponseTypeDef,
     StopImportResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     UpdateTrailResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -243,15 +243,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_channel)
         """
 
     async def create_event_data_store(
         self,
         *,
         Name: str,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...
@@ -498,16 +498,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_imports)
         """
 
     async def list_public_keys(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...
     ) -> ListPublicKeysResponseTypeDef:
         """
         Returns all public keys whose private keys were used to sign the digest files
         within the specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)
@@ -516,16 +516,16 @@
 
     async def list_queries(
         self,
         *,
         EventDataStore: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         QueryStatus: QueryStatusType = ...
     ) -> ListQueriesResponseTypeDef:
         """
         Returns a list of queries and query statuses for the past seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_queries)
@@ -550,16 +550,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_trails)
         """
 
     async def lookup_events(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> LookupEventsResponseTypeDef:
         """
         Looks up [management
         events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
@@ -571,16 +571,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#lookup_events)
         """
 
     async def put_event_selectors(
         self,
         *,
         TrailName: str,
-        EventSelectors: Sequence[EventSelectorTypeDef] = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...
+        EventSelectors: Sequence[EventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#put_event_selectors)
         """
@@ -649,16 +649,16 @@
         """
 
     async def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
-        StartEventTime: Union[datetime, str] = ...,
-        EndEventTime: Union[datetime, str] = ...,
+        StartEventTime: TimestampTypeDef = ...,
+        EndEventTime: TimestampTypeDef = ...,
         ImportId: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts an import of logged trail events from a source S3 bucket to a destination
         event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)
@@ -726,15 +726,15 @@
         """
 
     async def update_event_data_store(
         self,
         *,
         EventDataStore: str,
         Name: str = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/client.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,39 +11,38 @@
 
     session = get_session()
     async with session.create_client("cloudtrail") as client:
         client: CloudTrailClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ImportStatusType, QueryStatusType
 from .paginator import (
     ListImportFailuresPaginator,
     ListImportsPaginator,
     ListPublicKeysPaginator,
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 from .type_defs import (
-    AdvancedEventSelectorTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     CancelQueryResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     CreateTrailResponseTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     DestinationTypeDef,
-    EventSelectorTypeDef,
+    EventSelectorUnionTypeDef,
     GetChannelResponseTypeDef,
     GetEventDataStoreResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     GetImportResponseTypeDef,
     GetInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
@@ -65,14 +64,15 @@
     PutInsightSelectorsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     StartImportResponseTypeDef,
     StartQueryResponseTypeDef,
     StopImportResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     UpdateTrailResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -233,15 +233,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_channel)
         """
     async def create_event_data_store(
         self,
         *,
         Name: str,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...
@@ -465,16 +465,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_imports)
         """
     async def list_public_keys(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...
     ) -> ListPublicKeysResponseTypeDef:
         """
         Returns all public keys whose private keys were used to sign the digest files
         within the specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)
@@ -482,16 +482,16 @@
         """
     async def list_queries(
         self,
         *,
         EventDataStore: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         QueryStatus: QueryStatusType = ...
     ) -> ListQueriesResponseTypeDef:
         """
         Returns a list of queries and query statuses for the past seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_queries)
@@ -513,16 +513,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_trails)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_trails)
         """
     async def lookup_events(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> LookupEventsResponseTypeDef:
         """
         Looks up [management
         events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
@@ -533,16 +533,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.lookup_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#lookup_events)
         """
     async def put_event_selectors(
         self,
         *,
         TrailName: str,
-        EventSelectors: Sequence[EventSelectorTypeDef] = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...
+        EventSelectors: Sequence[EventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#put_event_selectors)
         """
@@ -604,16 +604,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#start_event_data_store_ingestion)
         """
     async def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
-        StartEventTime: Union[datetime, str] = ...,
-        EndEventTime: Union[datetime, str] = ...,
+        StartEventTime: TimestampTypeDef = ...,
+        EndEventTime: TimestampTypeDef = ...,
         ImportId: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts an import of logged trail events from a source S3 bucket to a destination
         event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)
@@ -674,15 +674,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#update_channel)
         """
     async def update_event_data_store(
         self,
         *,
         EventDataStore: str,
         Name: str = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/literals.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/literals.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/paginator.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
         list_public_keys_paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")
         list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
         list_trails_paginator: ListTrailsPaginator = client.get_paginator("list_trails")
         lookup_events_paginator: LookupEventsPaginator = client.get_paginator("lookup_events")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ImportStatusType
 from .type_defs import (
     ListImportFailuresResponseTypeDef,
     ListImportsResponseTypeDef,
     ListPublicKeysResponseTypeDef,
     ListTagsResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupAttributeTypeDef,
     LookupEventsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -78,15 +78,15 @@
 class ListImportFailuresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportfailurespaginator)
     """
 
     def paginate(
-        self, *, ImportId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ImportId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportFailuresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportfailurespaginator)
         """
 
 
@@ -97,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportspaginator)
         """
 
 
@@ -114,47 +114,47 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listpublickeyspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 
 class ListTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceIdList: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceIdList: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtagspaginator)
         """
 
 
 class ListTrailsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtrailspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtrailspaginator)
         """
 
 
@@ -164,16 +164,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#lookupeventspaginator)
     """
 
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/paginator.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,30 @@
         list_public_keys_paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")
         list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
         list_trails_paginator: ListTrailsPaginator = client.get_paginator("list_trails")
         lookup_events_paginator: LookupEventsPaginator = client.get_paginator("lookup_events")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ImportStatusType
 from .type_defs import (
     ListImportFailuresResponseTypeDef,
     ListImportsResponseTypeDef,
     ListPublicKeysResponseTypeDef,
     ListTagsResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupAttributeTypeDef,
     LookupEventsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -74,15 +74,15 @@
 class ListImportFailuresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportfailurespaginator)
     """
 
     def paginate(
-        self, *, ImportId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ImportId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportFailuresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportfailurespaginator)
         """
 
 class ListImportsPaginator(AioPaginator):
@@ -92,15 +92,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportspaginator)
         """
 
 class ListPublicKeysPaginator(AioPaginator):
@@ -108,45 +108,45 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listpublickeyspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 class ListTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceIdList: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceIdList: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtagspaginator)
         """
 
 class ListTrailsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtrailspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listtrailspaginator)
         """
 
 class LookupEventsPaginator(AioPaginator):
@@ -155,16 +155,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#lookupeventspaginator)
     """
 
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/type_defs.py` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudtrail.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,20 +35,21 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
+    "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
-    "CreateTrailResponseTypeDef",
+    "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -63,99 +64,105 @@
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
     "InsightSelectorTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
-    "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
-    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
-    "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    "ListPublicKeysRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PublicKeyTypeDef",
-    "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreEventDataStoreRequestRequestTypeDef",
     "StartEventDataStoreIngestionRequestRequestTypeDef",
     "StartLoggingRequestRequestTypeDef",
     "StartQueryRequestRequestTypeDef",
-    "StartQueryResponseTypeDef",
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
-    "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "ResourceTagTypeDef",
+    "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateTrailResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetTrailStatusResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartQueryResponseTypeDef",
+    "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
+    "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
     "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
+    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "ListImportsRequestListImportsPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    "ListPublicKeysRequestRequestTypeDef",
+    "ListQueriesRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
+    "AdvancedEventSelectorUnionTypeDef",
     "GetEventSelectorsResponseTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
     "PutEventSelectorsResponseTypeDef",
+    "EventSelectorUnionTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -169,14 +176,40 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+_RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Field": str,
+    },
+)
+_OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Equals": List[str],
+        "StartsWith": List[str],
+        "EndsWith": List[str],
+        "NotEquals": List[str],
+        "NotStartsWith": List[str],
+        "NotEndsWith": List[str],
+    },
+    total=False,
+)
+
+
+class AdvancedFieldSelectorOutputTypeDef(
+    _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
+):
+    pass
+
+
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -216,20 +249,22 @@
 
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
 ):
     pass
 
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "QueryId": str,
-        "QueryStatus": QueryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": str,
@@ -242,39 +277,28 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
-CreateTrailResponseTypeDef = TypedDict(
-    "CreateTrailResponseTypeDef",
+DataResourceOutputTypeDef = TypedDict(
+    "DataResourceOutputTypeDef",
     {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": str,
+        "Values": List[str],
     },
+    total=False,
 )
 
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
-        "Values": List[str],
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
@@ -476,61 +500,28 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrailRequestRequestTypeDef = TypedDict(
     "GetTrailRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 GetTrailStatusRequestRequestTypeDef = TypedDict(
     "GetTrailStatusRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetTrailStatusResponseTypeDef = TypedDict(
-    "GetTrailStatusResponseTypeDef",
-    {
-        "IsLogging": bool,
-        "LatestDeliveryError": str,
-        "LatestNotificationError": str,
-        "LatestDeliveryTime": datetime,
-        "LatestNotificationTime": datetime,
-        "StartLoggingTime": datetime,
-        "StopLoggingTime": datetime,
-        "LatestCloudWatchLogsDeliveryError": str,
-        "LatestCloudWatchLogsDeliveryTime": datetime,
-        "LatestDigestDeliveryTime": datetime,
-        "LatestDigestDeliveryError": str,
-        "LatestDeliveryAttemptTime": str,
-        "LatestNotificationAttemptTime": str,
-        "LatestNotificationAttemptSucceeded": str,
-        "LatestDeliveryAttemptSucceeded": str,
-        "TimeLoggingStarted": str,
-        "TimeLoggingStopped": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImportFailureListItemTypeDef = TypedDict(
     "ImportFailureListItemTypeDef",
     {
         "Location": str,
         "Status": ImportFailureStatusType,
         "ErrorType": str,
         "ErrorMessage": str,
@@ -574,36 +565,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "ImportId": str,
-    },
-)
-_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
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
 
-
-class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
-    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListImportFailuresRequestRequestTypeDef = TypedDict(
     "_RequiredListImportFailuresRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
 _OptionalListImportFailuresRequestRequestTypeDef = TypedDict(
@@ -619,122 +598,47 @@
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
 
-ListImportsRequestListImportsPaginateTypeDef = TypedDict(
-    "ListImportsRequestListImportsPaginateTypeDef",
-    {
-        "Destination": str,
-        "ImportStatus": ImportStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListPublicKeysRequestRequestTypeDef = TypedDict(
-    "ListPublicKeysRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Value": bytes,
         "ValidityStartTime": datetime,
         "ValidityEndTime": datetime,
         "Fingerprint": str,
     },
     total=False,
 )
 
-_RequiredListQueriesRequestRequestTypeDef = TypedDict(
-    "_RequiredListQueriesRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalListQueriesRequestRequestTypeDef = TypedDict(
-    "_OptionalListQueriesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "QueryStatus": QueryStatusType,
-    },
-    total=False,
-)
-
-
-class ListQueriesRequestRequestTypeDef(
-    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
-):
-    pass
-
-
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceIdList": Sequence[str],
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -748,22 +652,14 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
 
-ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
-    "ListTrailsRequestListTrailsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -782,59 +678,29 @@
     "LookupAttributeTypeDef",
     {
         "AttributeKey": LookupAttributeKeyType,
         "AttributeValue": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourcePolicy": str,
     },
 )
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "MemberAccountId": str,
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
 RestoreEventDataStoreRequestRequestTypeDef = TypedDict(
     "RestoreEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -859,22 +725,14 @@
         "DeliveryS3Uri": str,
         "QueryAlias": str,
         "QueryParameters": Sequence[str],
     },
     total=False,
 )
 
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -918,34 +776,14 @@
 
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTrailResponseTypeDef = TypedDict(
-    "UpdateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -994,14 +832,35 @@
     {
         "ResourceId": str,
         "TagsList": List[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedEventSelectorOutputTypeDef",
+    {
+        "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
+    },
+)
+_OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedEventSelectorOutputTypeDef",
+    {
+        "Name": str,
+    },
+    total=False,
+)
+
+
+class AdvancedEventSelectorOutputTypeDef(
+    _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
+):
+    pass
+
+
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
@@ -1015,20 +874,119 @@
 
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
 
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "QueryStatus": QueryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrailResponseTypeDef = TypedDict(
+    "CreateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrailStatusResponseTypeDef = TypedDict(
+    "GetTrailStatusResponseTypeDef",
+    {
+        "IsLogging": bool,
+        "LatestDeliveryError": str,
+        "LatestNotificationError": str,
+        "LatestDeliveryTime": datetime,
+        "LatestNotificationTime": datetime,
+        "StartLoggingTime": datetime,
+        "StopLoggingTime": datetime,
+        "LatestCloudWatchLogsDeliveryError": str,
+        "LatestCloudWatchLogsDeliveryTime": datetime,
+        "LatestDigestDeliveryTime": datetime,
+        "LatestDigestDeliveryError": str,
+        "LatestDeliveryAttemptTime": str,
+        "LatestNotificationAttemptTime": str,
+        "LatestNotificationAttemptSucceeded": str,
+        "LatestDeliveryAttemptSucceeded": str,
+        "TimeLoggingStarted": str,
+        "TimeLoggingStopped": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrailResponseTypeDef = TypedDict(
+    "UpdateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Name": str,
@@ -1055,15 +1013,15 @@
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
@@ -1088,56 +1046,67 @@
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EventSelectorOutputTypeDef = TypedDict(
+    "EventSelectorOutputTypeDef",
+    {
+        "ReadWriteType": ReadWriteTypeType,
+        "IncludeManagementEvents": bool,
+        "DataResources": List[DataResourceOutputTypeDef],
+        "ExcludeManagementEventSources": List[str],
+    },
+    total=False,
+)
+
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
-        "DataResources": List[DataResourceTypeDef],
-        "ExcludeManagementEventSources": List[str],
+        "DataResources": Sequence[DataResourceTypeDef],
+        "ExcludeManagementEventSources": Sequence[str],
     },
     total=False,
 )
 
 DescribeQueryResponseTypeDef = TypedDict(
     "DescribeQueryResponseTypeDef",
     {
         "QueryId": str,
         "QueryString": str,
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsForDescribeQueryTypeDef,
         "ErrorMessage": str,
         "DeliveryS3Uri": str,
         "DeliveryStatus": DeliveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrailsResponseTypeDef = TypedDict(
     "DescribeTrailsResponseTypeDef",
     {
         "trailList": List[TrailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrailResponseTypeDef = TypedDict(
     "GetTrailResponseTypeDef",
     {
         "Trail": TrailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
@@ -1154,15 +1123,15 @@
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutInsightSelectorsRequestRequestTypeDef = TypedDict(
     "PutInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1171,36 +1140,36 @@
 )
 
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsTypeDef,
         "QueryResultRows": List[List[Dict[str, str]]],
         "NextToken": str,
         "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportFailuresResponseTypeDef = TypedDict(
     "ListImportFailuresResponseTypeDef",
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
@@ -1208,135 +1177,212 @@
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "ImportId": str,
+    },
+)
+_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
+    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
+):
+    pass
+
+
+ListImportsRequestListImportsPaginateTypeDef = TypedDict(
+    "ListImportsRequestListImportsPaginateTypeDef",
+    {
+        "Destination": str,
+        "ImportStatus": ImportStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceIdList": Sequence[str],
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+
+ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestRequestTypeDef = TypedDict(
+    "ListPublicKeysRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListQueriesRequestRequestTypeDef = TypedDict(
+    "_RequiredListQueriesRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
     },
 )
+_OptionalListQueriesRequestRequestTypeDef = TypedDict(
+    "_OptionalListQueriesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "QueryStatus": QueryStatusType,
+    },
+    total=False,
+)
+
+
+class ListQueriesRequestRequestTypeDef(
+    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
+):
+    pass
+
 
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueriesResponseTypeDef = TypedDict(
     "ListQueriesResponseTypeDef",
     {
         "Queries": List[QueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrailsResponseTypeDef = TypedDict(
     "ListTrailsResponseTypeDef",
     {
         "Trails": List[TrailInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "ResourceTagList": List[ResourceTagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "TerminationProtectionEnabled": bool,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
@@ -1344,147 +1390,101 @@
 
 GetEventDataStoreResponseTypeDef = TypedDict(
     "GetEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-    },
-    total=False,
-)
-
-_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "KmsKeyId": str,
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
     },
     total=False,
 )
 
-
-class UpdateEventDataStoreRequestRequestTypeDef(
-    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
-    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateEventDataStoreResponseTypeDef = TypedDict(
     "UpdateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AdvancedEventSelectorUnionTypeDef = Union[
+    AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef
+]
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-    },
-)
-_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventSelectorsRequestRequestTypeDef",
-    {
-        "EventSelectors": Sequence[EventSelectorTypeDef],
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-    },
-    total=False,
-)
-
-
-class PutEventSelectorsRequestRequestTypeDef(
-    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
-):
-    pass
-
-
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EventSelectorUnionTypeDef = Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1492,25 +1492,25 @@
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportRequestRequestTypeDef = TypedDict(
     "StartImportRequestRequestTypeDef",
     {
         "Destinations": Sequence[str],
         "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
+        "StartEventTime": TimestampTypeDef,
+        "EndEventTime": TimestampTypeDef,
         "ImportId": str,
     },
     total=False,
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
@@ -1519,15 +1519,15 @@
         "Destinations": List[str],
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1535,32 +1535,110 @@
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
     },
 )
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class UpdateEventDataStoreRequestRequestTypeDef(
+    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
+    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+    },
+)
+_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventSelectorsRequestRequestTypeDef",
+    {
+        "EventSelectors": Sequence[EventSelectorUnionTypeDef],
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class PutEventSelectorsRequestRequestTypeDef(
+    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail/type_defs.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudtrail.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -34,20 +34,21 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
+    "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
-    "CreateTrailResponseTypeDef",
+    "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -62,99 +63,105 @@
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
     "InsightSelectorTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
-    "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
-    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
-    "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    "ListPublicKeysRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PublicKeyTypeDef",
-    "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreEventDataStoreRequestRequestTypeDef",
     "StartEventDataStoreIngestionRequestRequestTypeDef",
     "StartLoggingRequestRequestTypeDef",
     "StartQueryRequestRequestTypeDef",
-    "StartQueryResponseTypeDef",
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
-    "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "ResourceTagTypeDef",
+    "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateTrailResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetTrailStatusResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartQueryResponseTypeDef",
+    "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
+    "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
     "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
+    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "ListImportsRequestListImportsPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    "ListPublicKeysRequestRequestTypeDef",
+    "ListQueriesRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
+    "AdvancedEventSelectorUnionTypeDef",
     "GetEventSelectorsResponseTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
     "PutEventSelectorsResponseTypeDef",
+    "EventSelectorUnionTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -166,14 +173,38 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+_RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Field": str,
+    },
+)
+_OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Equals": List[str],
+        "StartsWith": List[str],
+        "EndsWith": List[str],
+        "NotEquals": List[str],
+        "NotStartsWith": List[str],
+        "NotEndsWith": List[str],
+    },
+    total=False,
+)
+
+class AdvancedFieldSelectorOutputTypeDef(
+    _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
+):
+    pass
+
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -209,20 +240,22 @@
 )
 
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
 ):
     pass
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "QueryId": str,
-        "QueryStatus": QueryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": str,
@@ -235,39 +268,28 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
-CreateTrailResponseTypeDef = TypedDict(
-    "CreateTrailResponseTypeDef",
+DataResourceOutputTypeDef = TypedDict(
+    "DataResourceOutputTypeDef",
     {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": str,
+        "Values": List[str],
     },
+    total=False,
 )
 
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
-        "Values": List[str],
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
@@ -467,61 +489,28 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrailRequestRequestTypeDef = TypedDict(
     "GetTrailRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 GetTrailStatusRequestRequestTypeDef = TypedDict(
     "GetTrailStatusRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetTrailStatusResponseTypeDef = TypedDict(
-    "GetTrailStatusResponseTypeDef",
-    {
-        "IsLogging": bool,
-        "LatestDeliveryError": str,
-        "LatestNotificationError": str,
-        "LatestDeliveryTime": datetime,
-        "LatestNotificationTime": datetime,
-        "StartLoggingTime": datetime,
-        "StopLoggingTime": datetime,
-        "LatestCloudWatchLogsDeliveryError": str,
-        "LatestCloudWatchLogsDeliveryTime": datetime,
-        "LatestDigestDeliveryTime": datetime,
-        "LatestDigestDeliveryError": str,
-        "LatestDeliveryAttemptTime": str,
-        "LatestNotificationAttemptTime": str,
-        "LatestNotificationAttemptSucceeded": str,
-        "LatestDeliveryAttemptSucceeded": str,
-        "TimeLoggingStarted": str,
-        "TimeLoggingStopped": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImportFailureListItemTypeDef = TypedDict(
     "ImportFailureListItemTypeDef",
     {
         "Location": str,
         "Status": ImportFailureStatusType,
         "ErrorType": str,
         "ErrorMessage": str,
@@ -565,34 +554,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "ImportId": str,
-    },
-)
-_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
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
 
-class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
-    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
-):
-    pass
-
 _RequiredListImportFailuresRequestRequestTypeDef = TypedDict(
     "_RequiredListImportFailuresRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
 _OptionalListImportFailuresRequestRequestTypeDef = TypedDict(
@@ -606,118 +585,47 @@
 
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
-ListImportsRequestListImportsPaginateTypeDef = TypedDict(
-    "ListImportsRequestListImportsPaginateTypeDef",
-    {
-        "Destination": str,
-        "ImportStatus": ImportStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListPublicKeysRequestRequestTypeDef = TypedDict(
-    "ListPublicKeysRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Value": bytes,
         "ValidityStartTime": datetime,
         "ValidityEndTime": datetime,
         "Fingerprint": str,
     },
     total=False,
 )
 
-_RequiredListQueriesRequestRequestTypeDef = TypedDict(
-    "_RequiredListQueriesRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalListQueriesRequestRequestTypeDef = TypedDict(
-    "_OptionalListQueriesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "QueryStatus": QueryStatusType,
-    },
-    total=False,
-)
-
-class ListQueriesRequestRequestTypeDef(
-    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
-):
-    pass
-
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceIdList": Sequence[str],
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -729,22 +637,14 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
-    "ListTrailsRequestListTrailsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -763,59 +663,29 @@
     "LookupAttributeTypeDef",
     {
         "AttributeKey": LookupAttributeKeyType,
         "AttributeValue": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourcePolicy": str,
     },
 )
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "MemberAccountId": str,
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
 RestoreEventDataStoreRequestRequestTypeDef = TypedDict(
     "RestoreEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -840,22 +710,14 @@
         "DeliveryS3Uri": str,
         "QueryAlias": str,
         "QueryParameters": Sequence[str],
     },
     total=False,
 )
 
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -897,34 +759,14 @@
 )
 
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
-UpdateTrailResponseTypeDef = TypedDict(
-    "UpdateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -971,14 +813,33 @@
     {
         "ResourceId": str,
         "TagsList": List[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedEventSelectorOutputTypeDef",
+    {
+        "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
+    },
+)
+_OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedEventSelectorOutputTypeDef",
+    {
+        "Name": str,
+    },
+    total=False,
+)
+
+class AdvancedEventSelectorOutputTypeDef(
+    _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
+):
+    pass
+
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
@@ -990,20 +851,119 @@
 )
 
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "QueryStatus": QueryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrailResponseTypeDef = TypedDict(
+    "CreateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrailStatusResponseTypeDef = TypedDict(
+    "GetTrailStatusResponseTypeDef",
+    {
+        "IsLogging": bool,
+        "LatestDeliveryError": str,
+        "LatestNotificationError": str,
+        "LatestDeliveryTime": datetime,
+        "LatestNotificationTime": datetime,
+        "StartLoggingTime": datetime,
+        "StopLoggingTime": datetime,
+        "LatestCloudWatchLogsDeliveryError": str,
+        "LatestCloudWatchLogsDeliveryTime": datetime,
+        "LatestDigestDeliveryTime": datetime,
+        "LatestDigestDeliveryError": str,
+        "LatestDeliveryAttemptTime": str,
+        "LatestNotificationAttemptTime": str,
+        "LatestNotificationAttemptSucceeded": str,
+        "LatestDeliveryAttemptSucceeded": str,
+        "TimeLoggingStarted": str,
+        "TimeLoggingStopped": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrailResponseTypeDef = TypedDict(
+    "UpdateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Name": str,
@@ -1028,15 +988,15 @@
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
@@ -1059,56 +1019,67 @@
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EventSelectorOutputTypeDef = TypedDict(
+    "EventSelectorOutputTypeDef",
+    {
+        "ReadWriteType": ReadWriteTypeType,
+        "IncludeManagementEvents": bool,
+        "DataResources": List[DataResourceOutputTypeDef],
+        "ExcludeManagementEventSources": List[str],
     },
+    total=False,
 )
 
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
-        "DataResources": List[DataResourceTypeDef],
-        "ExcludeManagementEventSources": List[str],
+        "DataResources": Sequence[DataResourceTypeDef],
+        "ExcludeManagementEventSources": Sequence[str],
     },
     total=False,
 )
 
 DescribeQueryResponseTypeDef = TypedDict(
     "DescribeQueryResponseTypeDef",
     {
         "QueryId": str,
         "QueryString": str,
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsForDescribeQueryTypeDef,
         "ErrorMessage": str,
         "DeliveryS3Uri": str,
         "DeliveryStatus": DeliveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrailsResponseTypeDef = TypedDict(
     "DescribeTrailsResponseTypeDef",
     {
         "trailList": List[TrailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrailResponseTypeDef = TypedDict(
     "GetTrailResponseTypeDef",
     {
         "Trail": TrailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
@@ -1125,15 +1096,15 @@
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutInsightSelectorsRequestRequestTypeDef = TypedDict(
     "PutInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1142,36 +1113,36 @@
 )
 
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsTypeDef,
         "QueryResultRows": List[List[Dict[str, str]]],
         "NextToken": str,
         "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportFailuresResponseTypeDef = TypedDict(
     "ListImportFailuresResponseTypeDef",
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
@@ -1179,133 +1150,206 @@
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "ImportId": str,
+    },
+)
+_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
+    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
+):
+    pass
+
+ListImportsRequestListImportsPaginateTypeDef = TypedDict(
+    "ListImportsRequestListImportsPaginateTypeDef",
+    {
+        "Destination": str,
+        "ImportStatus": ImportStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceIdList": Sequence[str],
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestRequestTypeDef = TypedDict(
+    "ListPublicKeysRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListQueriesRequestRequestTypeDef = TypedDict(
+    "_RequiredListQueriesRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalListQueriesRequestRequestTypeDef = TypedDict(
+    "_OptionalListQueriesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "QueryStatus": QueryStatusType,
+    },
+    total=False,
+)
+
+class ListQueriesRequestRequestTypeDef(
+    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
+):
+    pass
+
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueriesResponseTypeDef = TypedDict(
     "ListQueriesResponseTypeDef",
     {
         "Queries": List[QueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrailsResponseTypeDef = TypedDict(
     "ListTrailsResponseTypeDef",
     {
         "Trails": List[TrailInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "ResourceTagList": List[ResourceTagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "TerminationProtectionEnabled": bool,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
@@ -1313,143 +1357,101 @@
 
 GetEventDataStoreResponseTypeDef = TypedDict(
     "GetEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-    },
-    total=False,
-)
-
-_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "KmsKeyId": str,
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
     },
     total=False,
 )
 
-class UpdateEventDataStoreRequestRequestTypeDef(
-    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
-    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
 UpdateEventDataStoreResponseTypeDef = TypedDict(
     "UpdateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AdvancedEventSelectorUnionTypeDef = Union[
+    AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef
+]
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventSelectorsRequestRequestTypeDef",
-    {
-        "EventSelectors": Sequence[EventSelectorTypeDef],
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-    },
-    total=False,
-)
-
-class PutEventSelectorsRequestRequestTypeDef(
-    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
-):
-    pass
 
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EventSelectorUnionTypeDef = Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1457,25 +1459,25 @@
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportRequestRequestTypeDef = TypedDict(
     "StartImportRequestRequestTypeDef",
     {
         "Destinations": Sequence[str],
         "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
+        "StartEventTime": TimestampTypeDef,
+        "EndEventTime": TimestampTypeDef,
         "ImportId": str,
     },
     total=False,
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
@@ -1484,15 +1486,15 @@
         "Destinations": List[str],
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1500,32 +1502,105 @@
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
     },
 )
+_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class UpdateEventDataStoreRequestRequestTypeDef(
+    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
+    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+    },
+)
+_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventSelectorsRequestRequestTypeDef",
+    {
+        "EventSelectors": Sequence[EventSelectorUnionTypeDef],
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+    },
+    total=False,
+)
+
+class PutEventSelectorsRequestRequestTypeDef(
+    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/PKG-INFO` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudtrail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudtrail type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudtrail"></a>
 
 # types-aiobotocore-cloudtrail
 
 [![PyPI - types-aiobotocore-cloudtrail](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudtrail?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudtrail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudTrail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [types-aiobotocore-cloudtrail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/).
 
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
@@ -334,30 +333,31 @@
 )
 
 
 def check_value(value: DeliveryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudtrail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudtrail.type_defs import (
     TagTypeDef,
+    AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
-    CreateTrailResponseTypeDef,
+    DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -372,103 +372,109 @@
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
     InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
-    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
-    ListPublicKeysRequestRequestTypeDef,
+    TimestampTypeDef,
     PublicKeyTypeDef,
-    ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
     StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
-    StartQueryResponseTypeDef,
     StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
-    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     ResourceTagTypeDef,
+    AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateTrailResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetTrailStatusResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartQueryResponseTypeDef,
+    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
     PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListPublicKeysRequestRequestTypeDef,
+    ListQueriesRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreResponseTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     GetEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
     PutEventSelectorsResponseTypeDef,
+    EventSelectorUnionTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt` & `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*


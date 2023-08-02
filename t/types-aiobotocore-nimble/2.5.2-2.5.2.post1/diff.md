# Comparing `tmp/types-aiobotocore-nimble-2.5.2.tar.gz` & `tmp/types-aiobotocore-nimble-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-nimble-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-nimble-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
```

## Comparing `types-aiobotocore-nimble-2.5.2.tar` & `types-aiobotocore-nimble-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.754603 types-aiobotocore-nimble-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-07-08 01:44:02.750603 types-aiobotocore-nimble-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23577 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.754603 types-aiobotocore-nimble-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.750603 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47143 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47063 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70126 2023-07-08 01:35:53.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70009 2023-07-08 01:35:52.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.750603 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.429511 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47158 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47078 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-08-02 14:44:10.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-08-02 14:44:09.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71705 2023-08-02 14:44:11.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71586 2023-08-02 14:44:10.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-nimble-2.5.2/LICENSE` & `types-aiobotocore-nimble-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/PKG-INFO` & `types-aiobotocore-nimble-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore nimble type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore nimble type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-nimble"></a>
 
 # types-aiobotocore-nimble
 
 [![PyPI - types-aiobotocore-nimble](https://img.shields.io/pypi/v/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-nimble?color=blue)](https://pypistats.org/packages/types-aiobotocore-nimble)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [types-aiobotocore-nimble docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/).
 
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
@@ -460,25 +459,26 @@
 )
 
 
 def check_value(value: AutomaticTerminationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_nimble.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
+    ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
     ComputeFarmConfigurationTypeDef,
     CreateStreamingImageRequestRequestTypeDef,
     CreateStreamingSessionRequestRequestTypeDef,
     CreateStreamingSessionStreamRequestRequestTypeDef,
     StreamingSessionStreamTypeDef,
     ScriptParameterKeyValueTypeDef,
@@ -508,40 +508,28 @@
     GetStudioComponentRequestRequestTypeDef,
     GetStudioMemberRequestRequestTypeDef,
     StudioMembershipTypeDef,
     GetStudioRequestRequestTypeDef,
     LaunchProfileInitializationScriptTypeDef,
     ValidationResultTypeDef,
     LicenseServiceConfigurationTypeDef,
-    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEulaAcceptancesRequestRequestTypeDef,
-    ListEulasRequestListEulasPaginateTypeDef,
     ListEulasRequestRequestTypeDef,
-    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     ListLaunchProfileMembersRequestRequestTypeDef,
-    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     ListLaunchProfilesRequestRequestTypeDef,
-    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     ListStreamingImagesRequestRequestTypeDef,
-    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     ListStreamingSessionBackupsRequestRequestTypeDef,
-    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     ListStreamingSessionsRequestRequestTypeDef,
-    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     ListStudioComponentsRequestRequestTypeDef,
-    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
     ListStudioMembersRequestRequestTypeDef,
-    ListStudiosRequestListStudiosPaginateTypeDef,
     ListStudiosRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SharedFileSystemConfigurationTypeDef,
     StartStreamingSessionRequestRequestTypeDef,
     StartStudioSSOConfigurationRepairRequestRequestTypeDef,
     StopStreamingSessionRequestRequestTypeDef,
     StreamConfigurationSessionBackupTypeDef,
     VolumeConfigurationTypeDef,
     StreamingSessionStorageRootTypeDef,
@@ -549,14 +537,16 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLaunchProfileMemberRequestRequestTypeDef,
     UpdateStreamingImageRequestRequestTypeDef,
     UpdateStudioRequestRequestTypeDef,
     AcceptEulasResponseTypeDef,
     ListEulaAcceptancesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ActiveDirectoryConfigurationOutputTypeDef,
     ActiveDirectoryConfigurationTypeDef,
     LaunchProfileInitializationActiveDirectoryTypeDef,
     CreateStreamingSessionStreamResponseTypeDef,
     GetStreamingSessionStreamResponseTypeDef,
     CreateStudioRequestRequestTypeDef,
     StudioTypeDef,
     GetEulaResponseTypeDef,
@@ -576,62 +566,75 @@
     GetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     GetStudioRequestStudioDeletedWaitTypeDef,
     GetStudioRequestStudioReadyWaitTypeDef,
     GetStreamingSessionBackupResponseTypeDef,
     ListStreamingSessionBackupsResponseTypeDef,
     GetStudioMemberResponseTypeDef,
     ListStudioMembersResponseTypeDef,
+    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    ListEulasRequestListEulasPaginateTypeDef,
+    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    ListStudiosRequestListStudiosPaginateTypeDef,
     PutLaunchProfileMembersRequestRequestTypeDef,
     PutStudioMembersRequestRequestTypeDef,
     StreamingSessionTypeDef,
+    StreamConfigurationSessionStorageOutputTypeDef,
     StreamConfigurationSessionStorageTypeDef,
     StreamingImageTypeDef,
+    StudioComponentConfigurationOutputTypeDef,
     StudioComponentConfigurationTypeDef,
     LaunchProfileInitializationTypeDef,
     CreateStudioResponseTypeDef,
     DeleteStudioResponseTypeDef,
     GetStudioResponseTypeDef,
     ListStudiosResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     UpdateStudioResponseTypeDef,
     CreateStreamingSessionResponseTypeDef,
     DeleteStreamingSessionResponseTypeDef,
     GetStreamingSessionResponseTypeDef,
     ListStreamingSessionsResponseTypeDef,
     StartStreamingSessionResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
-    StreamConfigurationCreateTypeDef,
     StreamConfigurationTypeDef,
+    StreamConfigurationCreateTypeDef,
     CreateStreamingImageResponseTypeDef,
     DeleteStreamingImageResponseTypeDef,
     GetStreamingImageResponseTypeDef,
     ListStreamingImagesResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
-    CreateStudioComponentRequestRequestTypeDef,
     StudioComponentTypeDef,
+    CreateStudioComponentRequestRequestTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     UpdateStudioComponentRequestRequestTypeDef,
     GetLaunchProfileInitializationResponseTypeDef,
+    LaunchProfileTypeDef,
     CreateLaunchProfileRequestRequestTypeDef,
     UpdateLaunchProfileRequestRequestTypeDef,
-    LaunchProfileTypeDef,
     CreateStudioComponentResponseTypeDef,
     DeleteStudioComponentResponseTypeDef,
     GetStudioComponentResponseTypeDef,
     ListStudioComponentsResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     CreateLaunchProfileResponseTypeDef,
     DeleteLaunchProfileResponseTypeDef,
     GetLaunchProfileDetailsResponseTypeDef,
     GetLaunchProfileResponseTypeDef,
     ListLaunchProfilesResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptEulasRequestRequestTypeDef:
+def get_value() -> AcceptEulasRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-nimble-2.5.2/README.md` & `types-aiobotocore-nimble-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-nimble"></a>
 
 # types-aiobotocore-nimble
 
 [![PyPI - types-aiobotocore-nimble](https://img.shields.io/pypi/v/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-nimble?color=blue)](https://pypistats.org/packages/types-aiobotocore-nimble)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [types-aiobotocore-nimble docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/).
 
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
@@ -427,25 +427,26 @@
 )
 
 
 def check_value(value: AutomaticTerminationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_nimble.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
+    ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
     ComputeFarmConfigurationTypeDef,
     CreateStreamingImageRequestRequestTypeDef,
     CreateStreamingSessionRequestRequestTypeDef,
     CreateStreamingSessionStreamRequestRequestTypeDef,
     StreamingSessionStreamTypeDef,
     ScriptParameterKeyValueTypeDef,
@@ -475,40 +476,28 @@
     GetStudioComponentRequestRequestTypeDef,
     GetStudioMemberRequestRequestTypeDef,
     StudioMembershipTypeDef,
     GetStudioRequestRequestTypeDef,
     LaunchProfileInitializationScriptTypeDef,
     ValidationResultTypeDef,
     LicenseServiceConfigurationTypeDef,
-    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEulaAcceptancesRequestRequestTypeDef,
-    ListEulasRequestListEulasPaginateTypeDef,
     ListEulasRequestRequestTypeDef,
-    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     ListLaunchProfileMembersRequestRequestTypeDef,
-    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     ListLaunchProfilesRequestRequestTypeDef,
-    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     ListStreamingImagesRequestRequestTypeDef,
-    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     ListStreamingSessionBackupsRequestRequestTypeDef,
-    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     ListStreamingSessionsRequestRequestTypeDef,
-    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     ListStudioComponentsRequestRequestTypeDef,
-    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
     ListStudioMembersRequestRequestTypeDef,
-    ListStudiosRequestListStudiosPaginateTypeDef,
     ListStudiosRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SharedFileSystemConfigurationTypeDef,
     StartStreamingSessionRequestRequestTypeDef,
     StartStudioSSOConfigurationRepairRequestRequestTypeDef,
     StopStreamingSessionRequestRequestTypeDef,
     StreamConfigurationSessionBackupTypeDef,
     VolumeConfigurationTypeDef,
     StreamingSessionStorageRootTypeDef,
@@ -516,14 +505,16 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLaunchProfileMemberRequestRequestTypeDef,
     UpdateStreamingImageRequestRequestTypeDef,
     UpdateStudioRequestRequestTypeDef,
     AcceptEulasResponseTypeDef,
     ListEulaAcceptancesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ActiveDirectoryConfigurationOutputTypeDef,
     ActiveDirectoryConfigurationTypeDef,
     LaunchProfileInitializationActiveDirectoryTypeDef,
     CreateStreamingSessionStreamResponseTypeDef,
     GetStreamingSessionStreamResponseTypeDef,
     CreateStudioRequestRequestTypeDef,
     StudioTypeDef,
     GetEulaResponseTypeDef,
@@ -543,62 +534,75 @@
     GetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     GetStudioRequestStudioDeletedWaitTypeDef,
     GetStudioRequestStudioReadyWaitTypeDef,
     GetStreamingSessionBackupResponseTypeDef,
     ListStreamingSessionBackupsResponseTypeDef,
     GetStudioMemberResponseTypeDef,
     ListStudioMembersResponseTypeDef,
+    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    ListEulasRequestListEulasPaginateTypeDef,
+    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    ListStudiosRequestListStudiosPaginateTypeDef,
     PutLaunchProfileMembersRequestRequestTypeDef,
     PutStudioMembersRequestRequestTypeDef,
     StreamingSessionTypeDef,
+    StreamConfigurationSessionStorageOutputTypeDef,
     StreamConfigurationSessionStorageTypeDef,
     StreamingImageTypeDef,
+    StudioComponentConfigurationOutputTypeDef,
     StudioComponentConfigurationTypeDef,
     LaunchProfileInitializationTypeDef,
     CreateStudioResponseTypeDef,
     DeleteStudioResponseTypeDef,
     GetStudioResponseTypeDef,
     ListStudiosResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     UpdateStudioResponseTypeDef,
     CreateStreamingSessionResponseTypeDef,
     DeleteStreamingSessionResponseTypeDef,
     GetStreamingSessionResponseTypeDef,
     ListStreamingSessionsResponseTypeDef,
     StartStreamingSessionResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
-    StreamConfigurationCreateTypeDef,
     StreamConfigurationTypeDef,
+    StreamConfigurationCreateTypeDef,
     CreateStreamingImageResponseTypeDef,
     DeleteStreamingImageResponseTypeDef,
     GetStreamingImageResponseTypeDef,
     ListStreamingImagesResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
-    CreateStudioComponentRequestRequestTypeDef,
     StudioComponentTypeDef,
+    CreateStudioComponentRequestRequestTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     UpdateStudioComponentRequestRequestTypeDef,
     GetLaunchProfileInitializationResponseTypeDef,
+    LaunchProfileTypeDef,
     CreateLaunchProfileRequestRequestTypeDef,
     UpdateLaunchProfileRequestRequestTypeDef,
-    LaunchProfileTypeDef,
     CreateStudioComponentResponseTypeDef,
     DeleteStudioComponentResponseTypeDef,
     GetStudioComponentResponseTypeDef,
     ListStudioComponentsResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     CreateLaunchProfileResponseTypeDef,
     DeleteLaunchProfileResponseTypeDef,
     GetLaunchProfileDetailsResponseTypeDef,
     GetLaunchProfileResponseTypeDef,
     ListLaunchProfilesResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptEulasRequestRequestTypeDef:
+def get_value() -> AcceptEulasRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-nimble-2.5.2/setup.py` & `types-aiobotocore-nimble-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-nimble",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with"
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
-    keywords="aiobotocore nimble type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore nimble type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_nimble": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/"
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.pyi` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__main__.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NimbleStudio 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.NimbleStudio 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
-    StudioComponentConfigurationTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     UpdateStudioResponseTypeDef,
@@ -269,15 +269,15 @@
     async def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -777,15 +777,15 @@
 
     async def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.pyi` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
-    StudioComponentConfigurationTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     UpdateStudioResponseTypeDef,
@@ -256,15 +256,15 @@
     async def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -721,15 +721,15 @@
         """
     async def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.pyi` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,190 +67,174 @@
     "ListStreamingSessionBackupsPaginator",
     "ListStreamingSessionsPaginator",
     "ListStudioComponentsPaginator",
     "ListStudioMembersPaginator",
     "ListStudiosPaginator",
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
 class ListEulaAcceptancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaacceptancespaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         eulaIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEulaAcceptancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaacceptancespaginator)
         """
 
-
 class ListEulasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaspaginator)
     """
 
     def paginate(
-        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEulasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaspaginator)
         """
 
-
 class ListLaunchProfileMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilememberspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        launchProfileId: str,
-        studioId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, launchProfileId: str, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchProfileMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilememberspaginator)
         """
 
-
 class ListLaunchProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         principalId: str = ...,
         states: Sequence[LaunchProfileStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilespaginator)
         """
 
-
 class ListStreamingImagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingimagespaginator)
     """
 
     def paginate(
-        self, *, studioId: str, owner: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, studioId: str, owner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingimagespaginator)
         """
 
-
 class ListStreamingSessionBackupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionbackupspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingSessionBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionbackupspaginator)
         """
 
-
 class ListStreamingSessionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionspaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         ownedBy: str = ...,
         sessionIds: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionspaginator)
         """
 
-
 class ListStudioComponentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiocomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         states: Sequence[StudioComponentStateType] = ...,
         types: Sequence[StudioComponentTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStudioComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiocomponentspaginator)
         """
 
-
 class ListStudioMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiomemberspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStudioMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiomemberspaginator)
         """
 
-
 class ListStudiosPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStudiosResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiospaginator)
         """
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.pyi` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,178 +67,186 @@
     "ListStreamingSessionBackupsPaginator",
     "ListStreamingSessionsPaginator",
     "ListStudioComponentsPaginator",
     "ListStudioMembersPaginator",
     "ListStudiosPaginator",
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
 class ListEulaAcceptancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaacceptancespaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         eulaIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEulaAcceptancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaacceptancespaginator)
         """
 
+
 class ListEulasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaspaginator)
     """
 
     def paginate(
-        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEulasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaspaginator)
         """
 
+
 class ListLaunchProfileMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilememberspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        launchProfileId: str,
-        studioId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, launchProfileId: str, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchProfileMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilememberspaginator)
         """
 
+
 class ListLaunchProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         principalId: str = ...,
         states: Sequence[LaunchProfileStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilespaginator)
         """
 
+
 class ListStreamingImagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingimagespaginator)
     """
 
     def paginate(
-        self, *, studioId: str, owner: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, studioId: str, owner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingimagespaginator)
         """
 
+
 class ListStreamingSessionBackupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionbackupspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingSessionBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionbackupspaginator)
         """
 
+
 class ListStreamingSessionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionspaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         ownedBy: str = ...,
         sessionIds: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionspaginator)
         """
 
+
 class ListStudioComponentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiocomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         states: Sequence[StudioComponentStateType] = ...,
         types: Sequence[StudioComponentTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStudioComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiocomponentspaginator)
         """
 
+
 class ListStudioMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiomemberspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStudioMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiomemberspaginator)
         """
 
+
 class ListStudiosPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStudiosResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiospaginator)
         """
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_nimble.type_defs import AcceptEulasRequestRequestTypeDef
 
-    data: AcceptEulasRequestRequestTypeDef = {...}
+    data: AcceptEulasRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AutomaticTerminationModeType,
     LaunchProfilePlatformType,
     LaunchProfileStateType,
     LaunchProfileStatusCodeType,
     LaunchProfileValidationStateType,
@@ -53,14 +53,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
+    "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
     "CreateStreamingSessionRequestRequestTypeDef",
     "CreateStreamingSessionStreamRequestRequestTypeDef",
     "StreamingSessionStreamTypeDef",
     "ScriptParameterKeyValueTypeDef",
@@ -90,40 +91,28 @@
     "GetStudioComponentRequestRequestTypeDef",
     "GetStudioMemberRequestRequestTypeDef",
     "StudioMembershipTypeDef",
     "GetStudioRequestRequestTypeDef",
     "LaunchProfileInitializationScriptTypeDef",
     "ValidationResultTypeDef",
     "LicenseServiceConfigurationTypeDef",
-    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEulaAcceptancesRequestRequestTypeDef",
-    "ListEulasRequestListEulasPaginateTypeDef",
     "ListEulasRequestRequestTypeDef",
-    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
     "ListLaunchProfileMembersRequestRequestTypeDef",
-    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
     "ListLaunchProfilesRequestRequestTypeDef",
-    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
     "ListStreamingImagesRequestRequestTypeDef",
-    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
     "ListStreamingSessionBackupsRequestRequestTypeDef",
-    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     "ListStreamingSessionsRequestRequestTypeDef",
-    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     "ListStudioComponentsRequestRequestTypeDef",
-    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
     "ListStudioMembersRequestRequestTypeDef",
-    "ListStudiosRequestListStudiosPaginateTypeDef",
     "ListStudiosRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NewLaunchProfileMemberTypeDef",
     "NewStudioMemberTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SharedFileSystemConfigurationTypeDef",
     "StartStreamingSessionRequestRequestTypeDef",
     "StartStudioSSOConfigurationRepairRequestRequestTypeDef",
     "StopStreamingSessionRequestRequestTypeDef",
     "StreamConfigurationSessionBackupTypeDef",
     "VolumeConfigurationTypeDef",
     "StreamingSessionStorageRootTypeDef",
@@ -131,14 +120,16 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLaunchProfileMemberRequestRequestTypeDef",
     "UpdateStreamingImageRequestRequestTypeDef",
     "UpdateStudioRequestRequestTypeDef",
     "AcceptEulasResponseTypeDef",
     "ListEulaAcceptancesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ActiveDirectoryConfigurationOutputTypeDef",
     "ActiveDirectoryConfigurationTypeDef",
     "LaunchProfileInitializationActiveDirectoryTypeDef",
     "CreateStreamingSessionStreamResponseTypeDef",
     "GetStreamingSessionStreamResponseTypeDef",
     "CreateStudioRequestRequestTypeDef",
     "StudioTypeDef",
     "GetEulaResponseTypeDef",
@@ -158,47 +149,60 @@
     "GetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     "GetStudioRequestStudioDeletedWaitTypeDef",
     "GetStudioRequestStudioReadyWaitTypeDef",
     "GetStreamingSessionBackupResponseTypeDef",
     "ListStreamingSessionBackupsResponseTypeDef",
     "GetStudioMemberResponseTypeDef",
     "ListStudioMembersResponseTypeDef",
+    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    "ListEulasRequestListEulasPaginateTypeDef",
+    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    "ListStudiosRequestListStudiosPaginateTypeDef",
     "PutLaunchProfileMembersRequestRequestTypeDef",
     "PutStudioMembersRequestRequestTypeDef",
     "StreamingSessionTypeDef",
+    "StreamConfigurationSessionStorageOutputTypeDef",
     "StreamConfigurationSessionStorageTypeDef",
     "StreamingImageTypeDef",
+    "StudioComponentConfigurationOutputTypeDef",
     "StudioComponentConfigurationTypeDef",
     "LaunchProfileInitializationTypeDef",
     "CreateStudioResponseTypeDef",
     "DeleteStudioResponseTypeDef",
     "GetStudioResponseTypeDef",
     "ListStudiosResponseTypeDef",
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     "UpdateStudioResponseTypeDef",
     "CreateStreamingSessionResponseTypeDef",
     "DeleteStreamingSessionResponseTypeDef",
     "GetStreamingSessionResponseTypeDef",
     "ListStreamingSessionsResponseTypeDef",
     "StartStreamingSessionResponseTypeDef",
     "StopStreamingSessionResponseTypeDef",
-    "StreamConfigurationCreateTypeDef",
     "StreamConfigurationTypeDef",
+    "StreamConfigurationCreateTypeDef",
     "CreateStreamingImageResponseTypeDef",
     "DeleteStreamingImageResponseTypeDef",
     "GetStreamingImageResponseTypeDef",
     "ListStreamingImagesResponseTypeDef",
     "UpdateStreamingImageResponseTypeDef",
-    "CreateStudioComponentRequestRequestTypeDef",
     "StudioComponentTypeDef",
+    "CreateStudioComponentRequestRequestTypeDef",
+    "StudioComponentConfigurationUnionTypeDef",
     "UpdateStudioComponentRequestRequestTypeDef",
     "GetLaunchProfileInitializationResponseTypeDef",
+    "LaunchProfileTypeDef",
     "CreateLaunchProfileRequestRequestTypeDef",
     "UpdateLaunchProfileRequestRequestTypeDef",
-    "LaunchProfileTypeDef",
     "CreateStudioComponentResponseTypeDef",
     "DeleteStudioComponentResponseTypeDef",
     "GetStudioComponentResponseTypeDef",
     "ListStudioComponentsResponseTypeDef",
     "UpdateStudioComponentResponseTypeDef",
     "CreateLaunchProfileResponseTypeDef",
     "DeleteLaunchProfileResponseTypeDef",
@@ -238,14 +242,25 @@
         "accepteeId": str,
         "eulaAcceptanceId": str,
         "eulaId": str,
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
 ActiveDirectoryComputerAttributeTypeDef = TypedDict(
     "ActiveDirectoryComputerAttributeTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
@@ -754,37 +769,24 @@
     "LicenseServiceConfigurationTypeDef",
     {
         "endpoint": str,
     },
     total=False,
 )
 
-_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
-    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEulaAcceptancesRequestRequestTypeDef = TypedDict(
     "_RequiredListEulaAcceptancesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListEulaAcceptancesRequestRequestTypeDef = TypedDict(
@@ -800,55 +802,23 @@
 class ListEulaAcceptancesRequestRequestTypeDef(
     _RequiredListEulaAcceptancesRequestRequestTypeDef,
     _OptionalListEulaAcceptancesRequestRequestTypeDef,
 ):
     pass
 
 
-ListEulasRequestListEulasPaginateTypeDef = TypedDict(
-    "ListEulasRequestListEulasPaginateTypeDef",
-    {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEulasRequestRequestTypeDef = TypedDict(
     "ListEulasRequestRequestTypeDef",
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "launchProfileId": str,
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
-    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfileMembersRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -865,38 +835,14 @@
 class ListLaunchProfileMembersRequestRequestTypeDef(
     _RequiredListLaunchProfileMembersRequestRequestTypeDef,
     _OptionalListLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "principalId": str,
-        "states": Sequence[LaunchProfileStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
-    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLaunchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestRequestTypeDef = TypedDict(
@@ -914,37 +860,14 @@
 class ListLaunchProfilesRequestRequestTypeDef(
     _RequiredListLaunchProfilesRequestRequestTypeDef,
     _OptionalListLaunchProfilesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "owner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
-    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStreamingImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestRequestTypeDef = TypedDict(
@@ -960,37 +883,14 @@
 class ListStreamingImagesRequestRequestTypeDef(
     _RequiredListStreamingImagesRequestRequestTypeDef,
     _OptionalListStreamingImagesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "ownedBy": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
-    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
@@ -1006,39 +906,14 @@
 class ListStreamingSessionBackupsRequestRequestTypeDef(
     _RequiredListStreamingSessionBackupsRequestRequestTypeDef,
     _OptionalListStreamingSessionBackupsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "createdBy": str,
-        "ownedBy": str,
-        "sessionIds": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
-    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStreamingSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestRequestTypeDef = TypedDict(
@@ -1056,38 +931,14 @@
 class ListStreamingSessionsRequestRequestTypeDef(
     _RequiredListStreamingSessionsRequestRequestTypeDef,
     _OptionalListStreamingSessionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "states": Sequence[StudioComponentStateType],
-        "types": Sequence[StudioComponentTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
-    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStudioComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestRequestTypeDef = TypedDict(
@@ -1105,36 +956,14 @@
 class ListStudioComponentsRequestRequestTypeDef(
     _RequiredListStudioComponentsRequestRequestTypeDef,
     _OptionalListStudioComponentsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
-    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestRequestTypeDef = TypedDict(
@@ -1149,22 +978,14 @@
 
 class ListStudioMembersRequestRequestTypeDef(
     _RequiredListStudioMembersRequestRequestTypeDef, _OptionalListStudioMembersRequestRequestTypeDef
 ):
     pass
 
 
-ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosRequestListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStudiosRequestRequestTypeDef = TypedDict(
     "ListStudiosRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1172,22 +993,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 NewLaunchProfileMemberTypeDef = TypedDict(
     "NewLaunchProfileMemberTypeDef",
     {
         "persona": Literal["USER"],
         "principalId": str,
     },
 )
@@ -1196,35 +1009,14 @@
     "NewStudioMemberTypeDef",
     {
         "persona": Literal["ADMINISTRATOR"],
         "principalId": str,
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
 SharedFileSystemConfigurationTypeDef = TypedDict(
     "SharedFileSystemConfigurationTypeDef",
     {
         "endpoint": str,
         "fileSystemId": str,
         "linuxMountPoint": str,
         "shareName": str,
@@ -1456,25 +1248,43 @@
     pass
 
 
 AcceptEulasResponseTypeDef = TypedDict(
     "AcceptEulasResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEulaAcceptancesResponseTypeDef = TypedDict(
     "ListEulaAcceptancesResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+ActiveDirectoryConfigurationOutputTypeDef = TypedDict(
+    "ActiveDirectoryConfigurationOutputTypeDef",
+    {
+        "computerAttributes": List[ActiveDirectoryComputerAttributeTypeDef],
+        "directoryId": str,
+        "organizationalUnitDistinguishedName": str,
     },
+    total=False,
 )
 
 ActiveDirectoryConfigurationTypeDef = TypedDict(
     "ActiveDirectoryConfigurationTypeDef",
     {
         "computerAttributes": Sequence[ActiveDirectoryComputerAttributeTypeDef],
         "directoryId": str,
@@ -1497,23 +1307,23 @@
     total=False,
 )
 
 CreateStreamingSessionStreamResponseTypeDef = TypedDict(
     "CreateStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingSessionStreamResponseTypeDef = TypedDict(
     "GetStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioRequestRequestTypeDef",
     {
         "adminRoleArn": str,
@@ -1562,49 +1372,49 @@
     total=False,
 )
 
 GetEulaResponseTypeDef = TypedDict(
     "GetEulaResponseTypeDef",
     {
         "eula": EulaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEulasResponseTypeDef = TypedDict(
     "ListEulasResponseTypeDef",
     {
         "eulas": List[EulaTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchProfileMemberResponseTypeDef = TypedDict(
     "GetLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchProfileMembersResponseTypeDef = TypedDict(
     "ListLaunchProfileMembersResponseTypeDef",
     {
         "members": List[LaunchProfileMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchProfileMemberResponseTypeDef = TypedDict(
     "UpdateLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "launchProfileId": str,
@@ -1878,42 +1688,246 @@
     pass
 
 
 GetStreamingSessionBackupResponseTypeDef = TypedDict(
     "GetStreamingSessionBackupResponseTypeDef",
     {
         "streamingSessionBackup": StreamingSessionBackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamingSessionBackupsResponseTypeDef = TypedDict(
     "ListStreamingSessionBackupsResponseTypeDef",
     {
         "nextToken": str,
         "streamingSessionBackups": List[StreamingSessionBackupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStudioMemberResponseTypeDef = TypedDict(
     "GetStudioMemberResponseTypeDef",
     {
         "member": StudioMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudioMembersResponseTypeDef = TypedDict(
     "ListStudioMembersResponseTypeDef",
     {
         "members": List[StudioMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
+    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+):
+    pass
+
+
+ListEulasRequestListEulasPaginateTypeDef = TypedDict(
+    "ListEulasRequestListEulasPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "launchProfileId": str,
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
+    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "principalId": str,
+        "states": Sequence[LaunchProfileStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
+    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "owner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
+    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "ownedBy": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
+    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "createdBy": str,
+        "ownedBy": str,
+        "sessionIds": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
+    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "states": Sequence[StudioComponentStateType],
+        "types": Sequence[StudioComponentTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
+    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
+    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
+):
+    pass
+
+
+ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosRequestListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredPutLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "launchProfileId": str,
@@ -1990,14 +2004,36 @@
         "updatedBy": str,
         "volumeConfiguration": VolumeConfigurationTypeDef,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
+_RequiredStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
+    "_RequiredStreamConfigurationSessionStorageOutputTypeDef",
+    {
+        "mode": List[Literal["UPLOAD"]],
+    },
+)
+_OptionalStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
+    "_OptionalStreamConfigurationSessionStorageOutputTypeDef",
+    {
+        "root": StreamingSessionStorageRootTypeDef,
+    },
+    total=False,
+)
+
+
+class StreamConfigurationSessionStorageOutputTypeDef(
+    _RequiredStreamConfigurationSessionStorageOutputTypeDef,
+    _OptionalStreamConfigurationSessionStorageOutputTypeDef,
+):
+    pass
+
+
 _RequiredStreamConfigurationSessionStorageTypeDef = TypedDict(
     "_RequiredStreamConfigurationSessionStorageTypeDef",
     {
         "mode": Sequence[Literal["UPLOAD"]],
     },
 )
 _OptionalStreamConfigurationSessionStorageTypeDef = TypedDict(
@@ -2032,14 +2068,25 @@
         "statusMessage": str,
         "streamingImageId": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+StudioComponentConfigurationOutputTypeDef = TypedDict(
+    "StudioComponentConfigurationOutputTypeDef",
+    {
+        "activeDirectoryConfiguration": ActiveDirectoryConfigurationOutputTypeDef,
+        "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
+        "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
+        "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
+    },
+    total=False,
+)
+
 StudioComponentConfigurationTypeDef = TypedDict(
     "StudioComponentConfigurationTypeDef",
     {
         "activeDirectoryConfiguration": ActiveDirectoryConfigurationTypeDef,
         "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
         "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
         "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
@@ -2063,207 +2110,234 @@
     total=False,
 )
 
 CreateStudioResponseTypeDef = TypedDict(
     "CreateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStudioResponseTypeDef = TypedDict(
     "DeleteStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStudioResponseTypeDef = TypedDict(
     "GetStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudiosResponseTypeDef = TypedDict(
     "ListStudiosResponseTypeDef",
     {
         "nextToken": str,
         "studios": List[StudioTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStudioSSOConfigurationRepairResponseTypeDef = TypedDict(
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStudioResponseTypeDef = TypedDict(
     "UpdateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingSessionResponseTypeDef = TypedDict(
     "CreateStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStreamingSessionResponseTypeDef = TypedDict(
     "DeleteStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingSessionResponseTypeDef = TypedDict(
     "GetStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamingSessionsResponseTypeDef = TypedDict(
     "ListStreamingSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessions": List[StreamingSessionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStreamingSessionResponseTypeDef = TypedDict(
     "StartStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopStreamingSessionResponseTypeDef = TypedDict(
     "StopStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStreamConfigurationCreateTypeDef = TypedDict(
-    "_RequiredStreamConfigurationCreateTypeDef",
+_RequiredStreamConfigurationTypeDef = TypedDict(
+    "_RequiredStreamConfigurationTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
-        "streamingImageIds": Sequence[str],
+        "ec2InstanceTypes": List[StreamingInstanceTypeType],
+        "streamingImageIds": List[str],
     },
 )
-_OptionalStreamConfigurationCreateTypeDef = TypedDict(
-    "_OptionalStreamConfigurationCreateTypeDef",
+_OptionalStreamConfigurationTypeDef = TypedDict(
+    "_OptionalStreamConfigurationTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
-        "sessionStorage": StreamConfigurationSessionStorageTypeDef,
+        "sessionStorage": StreamConfigurationSessionStorageOutputTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class StreamConfigurationCreateTypeDef(
-    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
+class StreamConfigurationTypeDef(
+    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
 
-_RequiredStreamConfigurationTypeDef = TypedDict(
-    "_RequiredStreamConfigurationTypeDef",
+_RequiredStreamConfigurationCreateTypeDef = TypedDict(
+    "_RequiredStreamConfigurationCreateTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": List[StreamingInstanceTypeType],
-        "streamingImageIds": List[str],
+        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
+        "streamingImageIds": Sequence[str],
     },
 )
-_OptionalStreamConfigurationTypeDef = TypedDict(
-    "_OptionalStreamConfigurationTypeDef",
+_OptionalStreamConfigurationCreateTypeDef = TypedDict(
+    "_OptionalStreamConfigurationCreateTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class StreamConfigurationTypeDef(
-    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
+class StreamConfigurationCreateTypeDef(
+    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
 ):
     pass
 
 
 CreateStreamingImageResponseTypeDef = TypedDict(
     "CreateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStreamingImageResponseTypeDef = TypedDict(
     "DeleteStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingImageResponseTypeDef = TypedDict(
     "GetStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamingImagesResponseTypeDef = TypedDict(
     "ListStreamingImagesResponseTypeDef",
     {
         "nextToken": str,
         "streamingImages": List[StreamingImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStreamingImageResponseTypeDef = TypedDict(
     "UpdateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StudioComponentTypeDef = TypedDict(
+    "StudioComponentTypeDef",
+    {
+        "arn": str,
+        "configuration": StudioComponentConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SecurityGroupIds": List[str],
+        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
+        "name": str,
+        "runtimeRoleArn": str,
+        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
+        "secureInitializationRoleArn": str,
+        "state": StudioComponentStateType,
+        "statusCode": StudioComponentStatusCodeType,
+        "statusMessage": str,
+        "studioComponentId": str,
+        "subtype": StudioComponentSubtypeType,
+        "tags": Dict[str, str],
+        "type": StudioComponentTypeType,
+        "updatedAt": datetime,
+        "updatedBy": str,
+    },
+    total=False,
+)
+
 _RequiredCreateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioComponentRequestRequestTypeDef",
     {
         "name": str,
         "studioId": str,
         "type": StudioComponentTypeType,
     },
@@ -2289,41 +2363,17 @@
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
 
-StudioComponentTypeDef = TypedDict(
-    "StudioComponentTypeDef",
-    {
-        "arn": str,
-        "configuration": StudioComponentConfigurationTypeDef,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SecurityGroupIds": List[str],
-        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
-        "name": str,
-        "runtimeRoleArn": str,
-        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
-        "secureInitializationRoleArn": str,
-        "state": StudioComponentStateType,
-        "statusCode": StudioComponentStatusCodeType,
-        "statusMessage": str,
-        "studioComponentId": str,
-        "subtype": StudioComponentSubtypeType,
-        "tags": Dict[str, str],
-        "type": StudioComponentTypeType,
-        "updatedAt": datetime,
-        "updatedBy": str,
-    },
-    total=False,
-)
-
+StudioComponentConfigurationUnionTypeDef = Union[
+    StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+]
 _RequiredUpdateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -2353,16 +2403,40 @@
     pass
 
 
 GetLaunchProfileInitializationResponseTypeDef = TypedDict(
     "GetLaunchProfileInitializationResponseTypeDef",
     {
         "launchProfileInitialization": LaunchProfileInitializationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LaunchProfileTypeDef = TypedDict(
+    "LaunchProfileTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SubnetIds": List[str],
+        "launchProfileId": str,
+        "launchProfileProtocolVersions": List[str],
+        "name": str,
+        "state": LaunchProfileStateType,
+        "statusCode": LaunchProfileStatusCodeType,
+        "statusMessage": str,
+        "streamConfiguration": StreamConfigurationTypeDef,
+        "studioComponentIds": List[str],
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "updatedBy": str,
+        "validationResults": List[ValidationResultTypeDef],
     },
+    total=False,
 )
 
 _RequiredCreateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchProfileRequestRequestTypeDef",
     {
         "ec2SubnetIds": Sequence[str],
         "launchProfileProtocolVersions": Sequence[str],
@@ -2414,122 +2488,98 @@
 class UpdateLaunchProfileRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
 
-LaunchProfileTypeDef = TypedDict(
-    "LaunchProfileTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SubnetIds": List[str],
-        "launchProfileId": str,
-        "launchProfileProtocolVersions": List[str],
-        "name": str,
-        "state": LaunchProfileStateType,
-        "statusCode": LaunchProfileStatusCodeType,
-        "statusMessage": str,
-        "streamConfiguration": StreamConfigurationTypeDef,
-        "studioComponentIds": List[str],
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "updatedBy": str,
-        "validationResults": List[ValidationResultTypeDef],
-    },
-    total=False,
-)
-
 CreateStudioComponentResponseTypeDef = TypedDict(
     "CreateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStudioComponentResponseTypeDef = TypedDict(
     "DeleteStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStudioComponentResponseTypeDef = TypedDict(
     "GetStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudioComponentsResponseTypeDef = TypedDict(
     "ListStudioComponentsResponseTypeDef",
     {
         "nextToken": str,
         "studioComponents": List[StudioComponentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStudioComponentResponseTypeDef = TypedDict(
     "UpdateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLaunchProfileResponseTypeDef = TypedDict(
     "CreateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLaunchProfileResponseTypeDef = TypedDict(
     "DeleteLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchProfileDetailsResponseTypeDef = TypedDict(
     "GetLaunchProfileDetailsResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
         "streamingImages": List[StreamingImageTypeDef],
         "studioComponentSummaries": List[StudioComponentSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchProfileResponseTypeDef = TypedDict(
     "GetLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchProfilesResponseTypeDef = TypedDict(
     "ListLaunchProfilesResponseTypeDef",
     {
         "launchProfiles": List[LaunchProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchProfileResponseTypeDef = TypedDict(
     "UpdateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.pyi` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_nimble.type_defs import AcceptEulasRequestRequestTypeDef
 
-    data: AcceptEulasRequestRequestTypeDef = {...}
+    data: AcceptEulasRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AutomaticTerminationModeType,
     LaunchProfilePlatformType,
     LaunchProfileStateType,
     LaunchProfileStatusCodeType,
     LaunchProfileValidationStateType,
@@ -52,14 +52,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
+    "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
     "CreateStreamingSessionRequestRequestTypeDef",
     "CreateStreamingSessionStreamRequestRequestTypeDef",
     "StreamingSessionStreamTypeDef",
     "ScriptParameterKeyValueTypeDef",
@@ -89,40 +90,28 @@
     "GetStudioComponentRequestRequestTypeDef",
     "GetStudioMemberRequestRequestTypeDef",
     "StudioMembershipTypeDef",
     "GetStudioRequestRequestTypeDef",
     "LaunchProfileInitializationScriptTypeDef",
     "ValidationResultTypeDef",
     "LicenseServiceConfigurationTypeDef",
-    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEulaAcceptancesRequestRequestTypeDef",
-    "ListEulasRequestListEulasPaginateTypeDef",
     "ListEulasRequestRequestTypeDef",
-    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
     "ListLaunchProfileMembersRequestRequestTypeDef",
-    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
     "ListLaunchProfilesRequestRequestTypeDef",
-    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
     "ListStreamingImagesRequestRequestTypeDef",
-    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
     "ListStreamingSessionBackupsRequestRequestTypeDef",
-    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     "ListStreamingSessionsRequestRequestTypeDef",
-    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     "ListStudioComponentsRequestRequestTypeDef",
-    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
     "ListStudioMembersRequestRequestTypeDef",
-    "ListStudiosRequestListStudiosPaginateTypeDef",
     "ListStudiosRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NewLaunchProfileMemberTypeDef",
     "NewStudioMemberTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SharedFileSystemConfigurationTypeDef",
     "StartStreamingSessionRequestRequestTypeDef",
     "StartStudioSSOConfigurationRepairRequestRequestTypeDef",
     "StopStreamingSessionRequestRequestTypeDef",
     "StreamConfigurationSessionBackupTypeDef",
     "VolumeConfigurationTypeDef",
     "StreamingSessionStorageRootTypeDef",
@@ -130,14 +119,16 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLaunchProfileMemberRequestRequestTypeDef",
     "UpdateStreamingImageRequestRequestTypeDef",
     "UpdateStudioRequestRequestTypeDef",
     "AcceptEulasResponseTypeDef",
     "ListEulaAcceptancesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ActiveDirectoryConfigurationOutputTypeDef",
     "ActiveDirectoryConfigurationTypeDef",
     "LaunchProfileInitializationActiveDirectoryTypeDef",
     "CreateStreamingSessionStreamResponseTypeDef",
     "GetStreamingSessionStreamResponseTypeDef",
     "CreateStudioRequestRequestTypeDef",
     "StudioTypeDef",
     "GetEulaResponseTypeDef",
@@ -157,47 +148,60 @@
     "GetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     "GetStudioRequestStudioDeletedWaitTypeDef",
     "GetStudioRequestStudioReadyWaitTypeDef",
     "GetStreamingSessionBackupResponseTypeDef",
     "ListStreamingSessionBackupsResponseTypeDef",
     "GetStudioMemberResponseTypeDef",
     "ListStudioMembersResponseTypeDef",
+    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    "ListEulasRequestListEulasPaginateTypeDef",
+    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    "ListStudiosRequestListStudiosPaginateTypeDef",
     "PutLaunchProfileMembersRequestRequestTypeDef",
     "PutStudioMembersRequestRequestTypeDef",
     "StreamingSessionTypeDef",
+    "StreamConfigurationSessionStorageOutputTypeDef",
     "StreamConfigurationSessionStorageTypeDef",
     "StreamingImageTypeDef",
+    "StudioComponentConfigurationOutputTypeDef",
     "StudioComponentConfigurationTypeDef",
     "LaunchProfileInitializationTypeDef",
     "CreateStudioResponseTypeDef",
     "DeleteStudioResponseTypeDef",
     "GetStudioResponseTypeDef",
     "ListStudiosResponseTypeDef",
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     "UpdateStudioResponseTypeDef",
     "CreateStreamingSessionResponseTypeDef",
     "DeleteStreamingSessionResponseTypeDef",
     "GetStreamingSessionResponseTypeDef",
     "ListStreamingSessionsResponseTypeDef",
     "StartStreamingSessionResponseTypeDef",
     "StopStreamingSessionResponseTypeDef",
-    "StreamConfigurationCreateTypeDef",
     "StreamConfigurationTypeDef",
+    "StreamConfigurationCreateTypeDef",
     "CreateStreamingImageResponseTypeDef",
     "DeleteStreamingImageResponseTypeDef",
     "GetStreamingImageResponseTypeDef",
     "ListStreamingImagesResponseTypeDef",
     "UpdateStreamingImageResponseTypeDef",
-    "CreateStudioComponentRequestRequestTypeDef",
     "StudioComponentTypeDef",
+    "CreateStudioComponentRequestRequestTypeDef",
+    "StudioComponentConfigurationUnionTypeDef",
     "UpdateStudioComponentRequestRequestTypeDef",
     "GetLaunchProfileInitializationResponseTypeDef",
+    "LaunchProfileTypeDef",
     "CreateLaunchProfileRequestRequestTypeDef",
     "UpdateLaunchProfileRequestRequestTypeDef",
-    "LaunchProfileTypeDef",
     "CreateStudioComponentResponseTypeDef",
     "DeleteStudioComponentResponseTypeDef",
     "GetStudioComponentResponseTypeDef",
     "ListStudioComponentsResponseTypeDef",
     "UpdateStudioComponentResponseTypeDef",
     "CreateLaunchProfileResponseTypeDef",
     "DeleteLaunchProfileResponseTypeDef",
@@ -235,14 +239,25 @@
         "accepteeId": str,
         "eulaAcceptanceId": str,
         "eulaId": str,
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
 ActiveDirectoryComputerAttributeTypeDef = TypedDict(
     "ActiveDirectoryComputerAttributeTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
@@ -729,35 +744,24 @@
     "LicenseServiceConfigurationTypeDef",
     {
         "endpoint": str,
     },
     total=False,
 )
 
-_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
-    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-):
-    pass
-
 _RequiredListEulaAcceptancesRequestRequestTypeDef = TypedDict(
     "_RequiredListEulaAcceptancesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListEulaAcceptancesRequestRequestTypeDef = TypedDict(
@@ -771,53 +775,23 @@
 
 class ListEulaAcceptancesRequestRequestTypeDef(
     _RequiredListEulaAcceptancesRequestRequestTypeDef,
     _OptionalListEulaAcceptancesRequestRequestTypeDef,
 ):
     pass
 
-ListEulasRequestListEulasPaginateTypeDef = TypedDict(
-    "ListEulasRequestListEulasPaginateTypeDef",
-    {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEulasRequestRequestTypeDef = TypedDict(
     "ListEulasRequestRequestTypeDef",
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "launchProfileId": str,
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
-    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfileMembersRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -832,36 +806,14 @@
 
 class ListLaunchProfileMembersRequestRequestTypeDef(
     _RequiredListLaunchProfileMembersRequestRequestTypeDef,
     _OptionalListLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "principalId": str,
-        "states": Sequence[LaunchProfileStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
-    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-):
-    pass
-
 _RequiredListLaunchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestRequestTypeDef = TypedDict(
@@ -877,35 +829,14 @@
 
 class ListLaunchProfilesRequestRequestTypeDef(
     _RequiredListLaunchProfilesRequestRequestTypeDef,
     _OptionalListLaunchProfilesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "owner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
-    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-):
-    pass
-
 _RequiredListStreamingImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestRequestTypeDef = TypedDict(
@@ -919,35 +850,14 @@
 
 class ListStreamingImagesRequestRequestTypeDef(
     _RequiredListStreamingImagesRequestRequestTypeDef,
     _OptionalListStreamingImagesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "ownedBy": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
-    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
@@ -961,37 +871,14 @@
 
 class ListStreamingSessionBackupsRequestRequestTypeDef(
     _RequiredListStreamingSessionBackupsRequestRequestTypeDef,
     _OptionalListStreamingSessionBackupsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "createdBy": str,
-        "ownedBy": str,
-        "sessionIds": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
-    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStreamingSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestRequestTypeDef = TypedDict(
@@ -1007,36 +894,14 @@
 
 class ListStreamingSessionsRequestRequestTypeDef(
     _RequiredListStreamingSessionsRequestRequestTypeDef,
     _OptionalListStreamingSessionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "states": Sequence[StudioComponentStateType],
-        "types": Sequence[StudioComponentTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
-    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStudioComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestRequestTypeDef = TypedDict(
@@ -1052,34 +917,14 @@
 
 class ListStudioComponentsRequestRequestTypeDef(
     _RequiredListStudioComponentsRequestRequestTypeDef,
     _OptionalListStudioComponentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
-    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestRequestTypeDef = TypedDict(
@@ -1092,22 +937,14 @@
 )
 
 class ListStudioMembersRequestRequestTypeDef(
     _RequiredListStudioMembersRequestRequestTypeDef, _OptionalListStudioMembersRequestRequestTypeDef
 ):
     pass
 
-ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosRequestListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStudiosRequestRequestTypeDef = TypedDict(
     "ListStudiosRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1115,22 +952,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 NewLaunchProfileMemberTypeDef = TypedDict(
     "NewLaunchProfileMemberTypeDef",
     {
         "persona": Literal["USER"],
         "principalId": str,
     },
 )
@@ -1139,35 +968,14 @@
     "NewStudioMemberTypeDef",
     {
         "persona": Literal["ADMINISTRATOR"],
         "principalId": str,
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
 SharedFileSystemConfigurationTypeDef = TypedDict(
     "SharedFileSystemConfigurationTypeDef",
     {
         "endpoint": str,
         "fileSystemId": str,
         "linuxMountPoint": str,
         "shareName": str,
@@ -1383,25 +1191,43 @@
 ):
     pass
 
 AcceptEulasResponseTypeDef = TypedDict(
     "AcceptEulasResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEulaAcceptancesResponseTypeDef = TypedDict(
     "ListEulaAcceptancesResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+ActiveDirectoryConfigurationOutputTypeDef = TypedDict(
+    "ActiveDirectoryConfigurationOutputTypeDef",
+    {
+        "computerAttributes": List[ActiveDirectoryComputerAttributeTypeDef],
+        "directoryId": str,
+        "organizationalUnitDistinguishedName": str,
     },
+    total=False,
 )
 
 ActiveDirectoryConfigurationTypeDef = TypedDict(
     "ActiveDirectoryConfigurationTypeDef",
     {
         "computerAttributes": Sequence[ActiveDirectoryComputerAttributeTypeDef],
         "directoryId": str,
@@ -1424,23 +1250,23 @@
     total=False,
 )
 
 CreateStreamingSessionStreamResponseTypeDef = TypedDict(
     "CreateStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingSessionStreamResponseTypeDef = TypedDict(
     "GetStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioRequestRequestTypeDef",
     {
         "adminRoleArn": str,
@@ -1487,49 +1313,49 @@
     total=False,
 )
 
 GetEulaResponseTypeDef = TypedDict(
     "GetEulaResponseTypeDef",
     {
         "eula": EulaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEulasResponseTypeDef = TypedDict(
     "ListEulasResponseTypeDef",
     {
         "eulas": List[EulaTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchProfileMemberResponseTypeDef = TypedDict(
     "GetLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchProfileMembersResponseTypeDef = TypedDict(
     "ListLaunchProfileMembersResponseTypeDef",
     {
         "members": List[LaunchProfileMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchProfileMemberResponseTypeDef = TypedDict(
     "UpdateLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "launchProfileId": str,
@@ -1779,42 +1605,230 @@
 ):
     pass
 
 GetStreamingSessionBackupResponseTypeDef = TypedDict(
     "GetStreamingSessionBackupResponseTypeDef",
     {
         "streamingSessionBackup": StreamingSessionBackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamingSessionBackupsResponseTypeDef = TypedDict(
     "ListStreamingSessionBackupsResponseTypeDef",
     {
         "nextToken": str,
         "streamingSessionBackups": List[StreamingSessionBackupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStudioMemberResponseTypeDef = TypedDict(
     "GetStudioMemberResponseTypeDef",
     {
         "member": StudioMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudioMembersResponseTypeDef = TypedDict(
     "ListStudioMembersResponseTypeDef",
     {
         "members": List[StudioMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
+    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+):
+    pass
+
+ListEulasRequestListEulasPaginateTypeDef = TypedDict(
+    "ListEulasRequestListEulasPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "launchProfileId": str,
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
+    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+):
+    pass
+
+_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "principalId": str,
+        "states": Sequence[LaunchProfileStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
+    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+):
+    pass
+
+_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "owner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
+    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+):
+    pass
+
+_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "ownedBy": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
+    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "createdBy": str,
+        "ownedBy": str,
+        "sessionIds": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
+    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "states": Sequence[StudioComponentStateType],
+        "types": Sequence[StudioComponentTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
+    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
+    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
+):
+    pass
+
+ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosRequestListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredPutLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "launchProfileId": str,
@@ -1887,14 +1901,34 @@
         "updatedBy": str,
         "volumeConfiguration": VolumeConfigurationTypeDef,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
+_RequiredStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
+    "_RequiredStreamConfigurationSessionStorageOutputTypeDef",
+    {
+        "mode": List[Literal["UPLOAD"]],
+    },
+)
+_OptionalStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
+    "_OptionalStreamConfigurationSessionStorageOutputTypeDef",
+    {
+        "root": StreamingSessionStorageRootTypeDef,
+    },
+    total=False,
+)
+
+class StreamConfigurationSessionStorageOutputTypeDef(
+    _RequiredStreamConfigurationSessionStorageOutputTypeDef,
+    _OptionalStreamConfigurationSessionStorageOutputTypeDef,
+):
+    pass
+
 _RequiredStreamConfigurationSessionStorageTypeDef = TypedDict(
     "_RequiredStreamConfigurationSessionStorageTypeDef",
     {
         "mode": Sequence[Literal["UPLOAD"]],
     },
 )
 _OptionalStreamConfigurationSessionStorageTypeDef = TypedDict(
@@ -1927,14 +1961,25 @@
         "statusMessage": str,
         "streamingImageId": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+StudioComponentConfigurationOutputTypeDef = TypedDict(
+    "StudioComponentConfigurationOutputTypeDef",
+    {
+        "activeDirectoryConfiguration": ActiveDirectoryConfigurationOutputTypeDef,
+        "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
+        "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
+        "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
+    },
+    total=False,
+)
+
 StudioComponentConfigurationTypeDef = TypedDict(
     "StudioComponentConfigurationTypeDef",
     {
         "activeDirectoryConfiguration": ActiveDirectoryConfigurationTypeDef,
         "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
         "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
         "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
@@ -1958,203 +2003,230 @@
     total=False,
 )
 
 CreateStudioResponseTypeDef = TypedDict(
     "CreateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStudioResponseTypeDef = TypedDict(
     "DeleteStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStudioResponseTypeDef = TypedDict(
     "GetStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudiosResponseTypeDef = TypedDict(
     "ListStudiosResponseTypeDef",
     {
         "nextToken": str,
         "studios": List[StudioTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStudioSSOConfigurationRepairResponseTypeDef = TypedDict(
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStudioResponseTypeDef = TypedDict(
     "UpdateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingSessionResponseTypeDef = TypedDict(
     "CreateStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStreamingSessionResponseTypeDef = TypedDict(
     "DeleteStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingSessionResponseTypeDef = TypedDict(
     "GetStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamingSessionsResponseTypeDef = TypedDict(
     "ListStreamingSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessions": List[StreamingSessionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStreamingSessionResponseTypeDef = TypedDict(
     "StartStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopStreamingSessionResponseTypeDef = TypedDict(
     "StopStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStreamConfigurationCreateTypeDef = TypedDict(
-    "_RequiredStreamConfigurationCreateTypeDef",
+_RequiredStreamConfigurationTypeDef = TypedDict(
+    "_RequiredStreamConfigurationTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
-        "streamingImageIds": Sequence[str],
+        "ec2InstanceTypes": List[StreamingInstanceTypeType],
+        "streamingImageIds": List[str],
     },
 )
-_OptionalStreamConfigurationCreateTypeDef = TypedDict(
-    "_OptionalStreamConfigurationCreateTypeDef",
+_OptionalStreamConfigurationTypeDef = TypedDict(
+    "_OptionalStreamConfigurationTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
-        "sessionStorage": StreamConfigurationSessionStorageTypeDef,
+        "sessionStorage": StreamConfigurationSessionStorageOutputTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-class StreamConfigurationCreateTypeDef(
-    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
+class StreamConfigurationTypeDef(
+    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-_RequiredStreamConfigurationTypeDef = TypedDict(
-    "_RequiredStreamConfigurationTypeDef",
+_RequiredStreamConfigurationCreateTypeDef = TypedDict(
+    "_RequiredStreamConfigurationCreateTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": List[StreamingInstanceTypeType],
-        "streamingImageIds": List[str],
+        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
+        "streamingImageIds": Sequence[str],
     },
 )
-_OptionalStreamConfigurationTypeDef = TypedDict(
-    "_OptionalStreamConfigurationTypeDef",
+_OptionalStreamConfigurationCreateTypeDef = TypedDict(
+    "_OptionalStreamConfigurationCreateTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-class StreamConfigurationTypeDef(
-    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
+class StreamConfigurationCreateTypeDef(
+    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
 ):
     pass
 
 CreateStreamingImageResponseTypeDef = TypedDict(
     "CreateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStreamingImageResponseTypeDef = TypedDict(
     "DeleteStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingImageResponseTypeDef = TypedDict(
     "GetStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamingImagesResponseTypeDef = TypedDict(
     "ListStreamingImagesResponseTypeDef",
     {
         "nextToken": str,
         "streamingImages": List[StreamingImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStreamingImageResponseTypeDef = TypedDict(
     "UpdateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StudioComponentTypeDef = TypedDict(
+    "StudioComponentTypeDef",
+    {
+        "arn": str,
+        "configuration": StudioComponentConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SecurityGroupIds": List[str],
+        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
+        "name": str,
+        "runtimeRoleArn": str,
+        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
+        "secureInitializationRoleArn": str,
+        "state": StudioComponentStateType,
+        "statusCode": StudioComponentStatusCodeType,
+        "statusMessage": str,
+        "studioComponentId": str,
+        "subtype": StudioComponentSubtypeType,
+        "tags": Dict[str, str],
+        "type": StudioComponentTypeType,
+        "updatedAt": datetime,
+        "updatedBy": str,
+    },
+    total=False,
+)
+
 _RequiredCreateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioComponentRequestRequestTypeDef",
     {
         "name": str,
         "studioId": str,
         "type": StudioComponentTypeType,
     },
@@ -2178,41 +2250,17 @@
 
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-StudioComponentTypeDef = TypedDict(
-    "StudioComponentTypeDef",
-    {
-        "arn": str,
-        "configuration": StudioComponentConfigurationTypeDef,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SecurityGroupIds": List[str],
-        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
-        "name": str,
-        "runtimeRoleArn": str,
-        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
-        "secureInitializationRoleArn": str,
-        "state": StudioComponentStateType,
-        "statusCode": StudioComponentStatusCodeType,
-        "statusMessage": str,
-        "studioComponentId": str,
-        "subtype": StudioComponentSubtypeType,
-        "tags": Dict[str, str],
-        "type": StudioComponentTypeType,
-        "updatedAt": datetime,
-        "updatedBy": str,
-    },
-    total=False,
-)
-
+StudioComponentConfigurationUnionTypeDef = Union[
+    StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+]
 _RequiredUpdateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -2240,16 +2288,40 @@
 ):
     pass
 
 GetLaunchProfileInitializationResponseTypeDef = TypedDict(
     "GetLaunchProfileInitializationResponseTypeDef",
     {
         "launchProfileInitialization": LaunchProfileInitializationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LaunchProfileTypeDef = TypedDict(
+    "LaunchProfileTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SubnetIds": List[str],
+        "launchProfileId": str,
+        "launchProfileProtocolVersions": List[str],
+        "name": str,
+        "state": LaunchProfileStateType,
+        "statusCode": LaunchProfileStatusCodeType,
+        "statusMessage": str,
+        "streamConfiguration": StreamConfigurationTypeDef,
+        "studioComponentIds": List[str],
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "updatedBy": str,
+        "validationResults": List[ValidationResultTypeDef],
     },
+    total=False,
 )
 
 _RequiredCreateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchProfileRequestRequestTypeDef",
     {
         "ec2SubnetIds": Sequence[str],
         "launchProfileProtocolVersions": Sequence[str],
@@ -2297,122 +2369,98 @@
 
 class UpdateLaunchProfileRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
-LaunchProfileTypeDef = TypedDict(
-    "LaunchProfileTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SubnetIds": List[str],
-        "launchProfileId": str,
-        "launchProfileProtocolVersions": List[str],
-        "name": str,
-        "state": LaunchProfileStateType,
-        "statusCode": LaunchProfileStatusCodeType,
-        "statusMessage": str,
-        "streamConfiguration": StreamConfigurationTypeDef,
-        "studioComponentIds": List[str],
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "updatedBy": str,
-        "validationResults": List[ValidationResultTypeDef],
-    },
-    total=False,
-)
-
 CreateStudioComponentResponseTypeDef = TypedDict(
     "CreateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteStudioComponentResponseTypeDef = TypedDict(
     "DeleteStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStudioComponentResponseTypeDef = TypedDict(
     "GetStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudioComponentsResponseTypeDef = TypedDict(
     "ListStudioComponentsResponseTypeDef",
     {
         "nextToken": str,
         "studioComponents": List[StudioComponentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStudioComponentResponseTypeDef = TypedDict(
     "UpdateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLaunchProfileResponseTypeDef = TypedDict(
     "CreateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLaunchProfileResponseTypeDef = TypedDict(
     "DeleteLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchProfileDetailsResponseTypeDef = TypedDict(
     "GetLaunchProfileDetailsResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
         "streamingImages": List[StreamingImageTypeDef],
         "studioComponentSummaries": List[StudioComponentSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchProfileResponseTypeDef = TypedDict(
     "GetLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchProfilesResponseTypeDef = TypedDict(
     "ListLaunchProfilesResponseTypeDef",
     {
         "launchProfiles": List[LaunchProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchProfileResponseTypeDef = TypedDict(
     "UpdateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.py` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.pyi` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/PKG-INFO` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore nimble type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore nimble type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-nimble"></a>
 
 # types-aiobotocore-nimble
 
 [![PyPI - types-aiobotocore-nimble](https://img.shields.io/pypi/v/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-nimble?color=blue)](https://pypistats.org/packages/types-aiobotocore-nimble)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [types-aiobotocore-nimble docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/).
 
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
@@ -460,25 +459,26 @@
 )
 
 
 def check_value(value: AutomaticTerminationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_nimble.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
+    ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
     ComputeFarmConfigurationTypeDef,
     CreateStreamingImageRequestRequestTypeDef,
     CreateStreamingSessionRequestRequestTypeDef,
     CreateStreamingSessionStreamRequestRequestTypeDef,
     StreamingSessionStreamTypeDef,
     ScriptParameterKeyValueTypeDef,
@@ -508,40 +508,28 @@
     GetStudioComponentRequestRequestTypeDef,
     GetStudioMemberRequestRequestTypeDef,
     StudioMembershipTypeDef,
     GetStudioRequestRequestTypeDef,
     LaunchProfileInitializationScriptTypeDef,
     ValidationResultTypeDef,
     LicenseServiceConfigurationTypeDef,
-    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEulaAcceptancesRequestRequestTypeDef,
-    ListEulasRequestListEulasPaginateTypeDef,
     ListEulasRequestRequestTypeDef,
-    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     ListLaunchProfileMembersRequestRequestTypeDef,
-    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     ListLaunchProfilesRequestRequestTypeDef,
-    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     ListStreamingImagesRequestRequestTypeDef,
-    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     ListStreamingSessionBackupsRequestRequestTypeDef,
-    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     ListStreamingSessionsRequestRequestTypeDef,
-    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     ListStudioComponentsRequestRequestTypeDef,
-    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
     ListStudioMembersRequestRequestTypeDef,
-    ListStudiosRequestListStudiosPaginateTypeDef,
     ListStudiosRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SharedFileSystemConfigurationTypeDef,
     StartStreamingSessionRequestRequestTypeDef,
     StartStudioSSOConfigurationRepairRequestRequestTypeDef,
     StopStreamingSessionRequestRequestTypeDef,
     StreamConfigurationSessionBackupTypeDef,
     VolumeConfigurationTypeDef,
     StreamingSessionStorageRootTypeDef,
@@ -549,14 +537,16 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLaunchProfileMemberRequestRequestTypeDef,
     UpdateStreamingImageRequestRequestTypeDef,
     UpdateStudioRequestRequestTypeDef,
     AcceptEulasResponseTypeDef,
     ListEulaAcceptancesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ActiveDirectoryConfigurationOutputTypeDef,
     ActiveDirectoryConfigurationTypeDef,
     LaunchProfileInitializationActiveDirectoryTypeDef,
     CreateStreamingSessionStreamResponseTypeDef,
     GetStreamingSessionStreamResponseTypeDef,
     CreateStudioRequestRequestTypeDef,
     StudioTypeDef,
     GetEulaResponseTypeDef,
@@ -576,62 +566,75 @@
     GetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     GetStudioRequestStudioDeletedWaitTypeDef,
     GetStudioRequestStudioReadyWaitTypeDef,
     GetStreamingSessionBackupResponseTypeDef,
     ListStreamingSessionBackupsResponseTypeDef,
     GetStudioMemberResponseTypeDef,
     ListStudioMembersResponseTypeDef,
+    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    ListEulasRequestListEulasPaginateTypeDef,
+    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    ListStudiosRequestListStudiosPaginateTypeDef,
     PutLaunchProfileMembersRequestRequestTypeDef,
     PutStudioMembersRequestRequestTypeDef,
     StreamingSessionTypeDef,
+    StreamConfigurationSessionStorageOutputTypeDef,
     StreamConfigurationSessionStorageTypeDef,
     StreamingImageTypeDef,
+    StudioComponentConfigurationOutputTypeDef,
     StudioComponentConfigurationTypeDef,
     LaunchProfileInitializationTypeDef,
     CreateStudioResponseTypeDef,
     DeleteStudioResponseTypeDef,
     GetStudioResponseTypeDef,
     ListStudiosResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     UpdateStudioResponseTypeDef,
     CreateStreamingSessionResponseTypeDef,
     DeleteStreamingSessionResponseTypeDef,
     GetStreamingSessionResponseTypeDef,
     ListStreamingSessionsResponseTypeDef,
     StartStreamingSessionResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
-    StreamConfigurationCreateTypeDef,
     StreamConfigurationTypeDef,
+    StreamConfigurationCreateTypeDef,
     CreateStreamingImageResponseTypeDef,
     DeleteStreamingImageResponseTypeDef,
     GetStreamingImageResponseTypeDef,
     ListStreamingImagesResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
-    CreateStudioComponentRequestRequestTypeDef,
     StudioComponentTypeDef,
+    CreateStudioComponentRequestRequestTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     UpdateStudioComponentRequestRequestTypeDef,
     GetLaunchProfileInitializationResponseTypeDef,
+    LaunchProfileTypeDef,
     CreateLaunchProfileRequestRequestTypeDef,
     UpdateLaunchProfileRequestRequestTypeDef,
-    LaunchProfileTypeDef,
     CreateStudioComponentResponseTypeDef,
     DeleteStudioComponentResponseTypeDef,
     GetStudioComponentResponseTypeDef,
     ListStudioComponentsResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     CreateLaunchProfileResponseTypeDef,
     DeleteLaunchProfileResponseTypeDef,
     GetLaunchProfileDetailsResponseTypeDef,
     GetLaunchProfileResponseTypeDef,
     ListLaunchProfilesResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptEulasRequestRequestTypeDef:
+def get_value() -> AcceptEulasRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/SOURCES.txt` & `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*


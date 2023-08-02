# Comparing `tmp/types-aiobotocore-codecatalyst-2.5.2.tar.gz` & `tmp/types-aiobotocore-codecatalyst-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecatalyst-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecatalyst-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codecatalyst-2.5.2.tar` & `types-aiobotocore-codecatalyst-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.849869 types-aiobotocore-codecatalyst-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-08 01:43:23.849869 types-aiobotocore-codecatalyst-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.849869 types-aiobotocore-codecatalyst-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.841869 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25836 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34784 2023-07-08 01:27:26.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34721 2023-07-08 01:27:26.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:25.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.849869 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-08 01:43:23.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:23.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:23.000000 types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.569625 types-aiobotocore-codecatalyst-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-08-02 14:52:02.557625 types-aiobotocore-codecatalyst-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.569625 types-aiobotocore-codecatalyst-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.557625 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25852 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-08-02 14:34:59.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-08-02 14:34:58.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-02 14:34:58.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-02 14:34:58.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-08-02 14:34:59.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34697 2023-08-02 14:34:59.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.557625 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/LICENSE` & `types-aiobotocore-codecatalyst-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2/PKG-INFO` & `types-aiobotocore-codecatalyst-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codecatalyst type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codecatalyst"></a>
 
 # types-aiobotocore-codecatalyst
 
 [![PyPI - types-aiobotocore-codecatalyst](https://img.shields.io/pypi/v/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codecatalyst?color=blue)](https://pypistats.org/packages/types-aiobotocore-codecatalyst)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeCatalyst 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
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
@@ -344,110 +343,111 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codecatalyst.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    TimestampTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
+    CreateAccessTokenRequestRequestTypeDef,
+    ListEventLogsRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessTokenSummaryTypeDef:
+def get_value() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/README.md` & `types-aiobotocore-codecatalyst-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codecatalyst"></a>
 
 # types-aiobotocore-codecatalyst
 
 [![PyPI - types-aiobotocore-codecatalyst](https://img.shields.io/pypi/v/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codecatalyst?color=blue)](https://pypistats.org/packages/types-aiobotocore-codecatalyst)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeCatalyst 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
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
@@ -311,110 +311,111 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codecatalyst.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    TimestampTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
+    CreateAccessTokenRequestRequestTypeDef,
+    ListEventLogsRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessTokenSummaryTypeDef:
+def get_value() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/setup.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecatalyst",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with"
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
-    keywords="aiobotocore codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codecatalyst type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codecatalyst": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/"
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/__init__.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/__init__.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/__main__.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCatalyst 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeCatalyst 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
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

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/client.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("codecatalyst") as client:
         client: CodeCatalystClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import InstanceTypeType
 from .paginator import (
     ListAccessTokensPaginator,
@@ -58,14 +57,15 @@
     PersistentStorageConfigurationTypeDef,
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
+    TimestampTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -123,15 +123,15 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#close)
         """
 
     async def create_access_token(
-        self, *, name: str, expiresTime: Union[datetime, str] = ...
+        self, *, name: str, expiresTime: TimestampTypeDef = ...
     ) -> CreateAccessTokenResponseTypeDef:
         """
         Creates a personal access token (PAT) for the current user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_access_token)
         """
@@ -316,16 +316,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_dev_environments)
         """
 
     async def list_event_logs(
         self,
         *,
         spaceName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         eventName: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListEventLogsResponseTypeDef:
         """
         Retrieves a list of events that occurred during a specified time period in a
         space.
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/client.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("codecatalyst") as client:
         client: CodeCatalystClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import InstanceTypeType
 from .paginator import (
     ListAccessTokensPaginator,
@@ -58,14 +57,15 @@
     PersistentStorageConfigurationTypeDef,
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
+    TimestampTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -116,15 +116,15 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#close)
         """
     async def create_access_token(
-        self, *, name: str, expiresTime: Union[datetime, str] = ...
+        self, *, name: str, expiresTime: TimestampTypeDef = ...
     ) -> CreateAccessTokenResponseTypeDef:
         """
         Creates a personal access token (PAT) for the current user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_access_token)
         """
@@ -293,16 +293,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_dev_environments)
         """
     async def list_event_logs(
         self,
         *,
         spaceName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         eventName: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListEventLogsResponseTypeDef:
         """
         Retrieves a list of events that occurred during a specified time period in a
         space.
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/literals.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/literals.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/paginator.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,15 @@
         list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
         list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
         list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
         list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
         list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     FilterTypeDef,
     ListAccessTokensResponseTypeDef,
@@ -48,14 +47,15 @@
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PaginatorConfigTypeDef,
     ProjectListFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListAccessTokensPaginator",
     "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
@@ -79,15 +79,15 @@
 class ListAccessTokensPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
 
@@ -99,15 +99,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 
@@ -119,15 +119,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 
@@ -137,18 +137,18 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listeventlogspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         eventName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 
@@ -159,30 +159,30 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listprojectspaginator)
         """
 
 
 class ListSourceRepositoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
 
@@ -194,28 +194,28 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 
 class ListSpacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/paginator.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,15 @@
         list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
         list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
         list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
         list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
         list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     FilterTypeDef,
     ListAccessTokensResponseTypeDef,
@@ -48,14 +47,15 @@
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PaginatorConfigTypeDef,
     ProjectListFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListAccessTokensPaginator",
     "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
@@ -76,15 +76,15 @@
 class ListAccessTokensPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
 class ListDevEnvironmentSessionsPaginator(AioPaginator):
@@ -95,15 +95,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 class ListDevEnvironmentsPaginator(AioPaginator):
@@ -114,15 +114,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 class ListEventLogsPaginator(AioPaginator):
@@ -131,18 +131,18 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listeventlogspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         eventName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
@@ -152,29 +152,29 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listprojectspaginator)
         """
 
 class ListSourceRepositoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
 class ListSourceRepositoryBranchesPaginator(AioPaginator):
@@ -185,27 +185,27 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 class ListSpacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/type_defs.py` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codecatalyst.type_defs import AccessTokenSummaryTypeDef
 
-    data: AccessTokenSummaryTypeDef = {...}
+    data: AccessTokenSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,87 +32,88 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
-    "CreateAccessTokenRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
+    "TimestampTypeDef",
+    "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
-    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSpaceRequestRequestTypeDef",
-    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
-    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
-    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
-    "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
+    "CreateAccessTokenRequestRequestTypeDef",
+    "ListEventLogsRequestRequestTypeDef",
+    "CreateAccessTokenResponseTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
+    "GetProjectResponseTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSpaceResponseTypeDef",
+    "GetSubscriptionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
+    "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "VerifySessionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
@@ -138,43 +139,23 @@
 
 class AccessTokenSummaryTypeDef(
     _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
 ):
     pass
 
 
-_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessTokenRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessTokenRequestRequestTypeDef",
-    {
-        "expiresTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class CreateAccessTokenRequestRequestTypeDef(
-    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
-):
-    pass
-
-
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+TimestampTypeDef = Union[datetime, str]
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -205,24 +186,14 @@
 )
 
 
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -237,25 +208,14 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -273,25 +233,14 @@
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    {
-        "ref": str,
-        "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -300,24 +249,14 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
@@ -473,126 +412,65 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    {
-        "https": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
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
 
 ListAccessTokensRequestRequestTypeDef = TypedDict(
     "ListAccessTokensRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "devEnvironmentId": str,
-    },
-)
-_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
-    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "devEnvironmentId": str,
     },
@@ -610,64 +488,14 @@
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestRequestTypeDef",
-    {
-        "eventName": str,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListEventLogsRequestRequestTypeDef(
-    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredProjectListFilterTypeDef = TypedDict(
     "_RequiredProjectListFilterTypeDef",
     {
         "key": Literal["hasAccessTo"],
         "values": Sequence[str],
     },
 )
@@ -726,37 +554,14 @@
 
 class ListSourceRepositoriesItemTypeDef(
     _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
 ):
     pass
 
 
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -784,38 +589,14 @@
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
     total=False,
 )
 
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -833,22 +614,14 @@
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -870,101 +643,218 @@
 )
 
 
 class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+    },
+)
+
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
+_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessTokenRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessTokenRequestRequestTypeDef",
+    {
+        "expiresTime": TimestampTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class CreateAccessTokenRequestRequestTypeDef(
+    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "spaceName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestRequestTypeDef",
+    {
+        "eventName": str,
+        "nextToken": str,
+        "maxResults": int,
     },
+    total=False,
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+
+class ListEventLogsRequestRequestTypeDef(
+    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
+):
+    pass
+
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
+    {
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    {
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    {
+        "https": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
+    {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "sessionId": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StopDevEnvironmentSessionResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
-    {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1025,15 +915,15 @@
         "spaceName": str,
         "projectName": str,
         "alias": str,
         "ides": List[IdeConfigurationTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1066,15 +956,15 @@
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -1097,15 +987,15 @@
 
 
 ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
     "ListDevEnvironmentSessionsResponseTypeDef",
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSummaryTypeDef = TypedDict(
     "_RequiredDevEnvironmentSummaryTypeDef",
     {
         "id": str,
@@ -1149,27 +1039,27 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEventLogEntryTypeDef = TypedDict(
     "_RequiredEventLogEntryTypeDef",
     {
         "id": str,
@@ -1197,74 +1087,186 @@
 )
 
 
 class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
     pass
 
 
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+):
+    pass
+
+
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+):
+    pass
+
+
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
@@ -1297,42 +1299,42 @@
 
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1343,19 +1345,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst/type_defs.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codecatalyst.type_defs import AccessTokenSummaryTypeDef
 
-    data: AccessTokenSummaryTypeDef = {...}
+    data: AccessTokenSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -31,87 +31,88 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
-    "CreateAccessTokenRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
+    "TimestampTypeDef",
+    "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
-    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSpaceRequestRequestTypeDef",
-    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
-    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
-    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
-    "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
+    "CreateAccessTokenRequestRequestTypeDef",
+    "ListEventLogsRequestRequestTypeDef",
+    "CreateAccessTokenResponseTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
+    "GetProjectResponseTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSpaceResponseTypeDef",
+    "GetSubscriptionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
+    "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "VerifySessionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
@@ -135,41 +136,23 @@
 )
 
 class AccessTokenSummaryTypeDef(
     _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
 ):
     pass
 
-_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessTokenRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessTokenRequestRequestTypeDef",
-    {
-        "expiresTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class CreateAccessTokenRequestRequestTypeDef(
-    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
-):
-    pass
-
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+TimestampTypeDef = Union[datetime, str]
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -198,24 +181,14 @@
     },
     total=False,
 )
 
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -228,25 +201,14 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -262,25 +224,14 @@
 
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    {
-        "ref": str,
-        "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -289,24 +240,14 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
@@ -454,124 +395,65 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    {
-        "https": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
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
 
 ListAccessTokensRequestRequestTypeDef = TypedDict(
     "ListAccessTokensRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "devEnvironmentId": str,
-    },
-)
-_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
-    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "devEnvironmentId": str,
     },
@@ -587,60 +469,14 @@
 
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestRequestTypeDef",
-    {
-        "eventName": str,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListEventLogsRequestRequestTypeDef(
-    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
-):
-    pass
-
 _RequiredProjectListFilterTypeDef = TypedDict(
     "_RequiredProjectListFilterTypeDef",
     {
         "key": Literal["hasAccessTo"],
         "values": Sequence[str],
     },
 )
@@ -693,35 +529,14 @@
 )
 
 class ListSourceRepositoriesItemTypeDef(
     _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
 ):
     pass
 
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -747,36 +562,14 @@
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
     total=False,
 )
 
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -792,22 +585,14 @@
 
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -827,101 +612,214 @@
     },
     total=False,
 )
 
 class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+    },
+)
+
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
+_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessTokenRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessTokenRequestRequestTypeDef",
+    {
+        "expiresTime": TimestampTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class CreateAccessTokenRequestRequestTypeDef(
+    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
+):
+    pass
+
+_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "spaceName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestRequestTypeDef",
+    {
+        "eventName": str,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListEventLogsRequestRequestTypeDef(
+    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
+):
+    pass
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
+    {
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    {
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    {
+        "https": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
+    {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "sessionId": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StopDevEnvironmentSessionResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
-    {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -978,15 +876,15 @@
         "spaceName": str,
         "projectName": str,
         "alias": str,
         "ides": List[IdeConfigurationTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1017,15 +915,15 @@
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -1046,15 +944,15 @@
     pass
 
 ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
     "ListDevEnvironmentSessionsResponseTypeDef",
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSummaryTypeDef = TypedDict(
     "_RequiredDevEnvironmentSummaryTypeDef",
     {
         "id": str,
@@ -1096,27 +994,27 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEventLogEntryTypeDef = TypedDict(
     "_RequiredEventLogEntryTypeDef",
     {
         "id": str,
@@ -1142,70 +1040,174 @@
     },
     total=False,
 )
 
 class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
     pass
 
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+):
+    pass
+
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
 ):
     pass
 
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
@@ -1234,42 +1236,42 @@
     pass
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1280,19 +1282,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/PKG-INFO` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codecatalyst type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codecatalyst"></a>
 
 # types-aiobotocore-codecatalyst
 
 [![PyPI - types-aiobotocore-codecatalyst](https://img.shields.io/pypi/v/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codecatalyst?color=blue)](https://pypistats.org/packages/types-aiobotocore-codecatalyst)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeCatalyst 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
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
@@ -344,110 +343,111 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codecatalyst.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    TimestampTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
+    CreateAccessTokenRequestRequestTypeDef,
+    ListEventLogsRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessTokenSummaryTypeDef:
+def get_value() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt` & `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-lex-models-2.5.2.tar.gz` & `tmp/types-aiobotocore-lex-models-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-models-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-models-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-lex-models-2.5.2.tar` & `types-aiobotocore-lex-models-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.338427 types-aiobotocore-lex-models-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-08 01:43:53.330427 types-aiobotocore-lex-models-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.338427 types-aiobotocore-lex-models-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:33:43.000000 types-aiobotocore-lex-models-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.330427 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37384 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37323 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-07-08 01:33:45.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46040 2023-07-08 01:33:45.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.330427 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.549543 types-aiobotocore-lex-models-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-08-02 14:52:33.541543 types-aiobotocore-lex-models-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.549543 types-aiobotocore-lex-models-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.541543 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37378 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37317 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49190 2023-08-02 14:41:52.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49130 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.541543 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-models-2.5.2/LICENSE` & `types-aiobotocore-lex-models-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2/PKG-INFO` & `types-aiobotocore-lex-models-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lex-models type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lex-models type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lex-models"></a>
 
 # types-aiobotocore-lex-models
 
 [![PyPI - types-aiobotocore-lex-models](https://img.shields.io/pypi/v/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [types-aiobotocore-lex-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/).
 
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
@@ -367,146 +366,158 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lex_models.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lex_models.type_defs import (
+    BlobTypeDef,
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     IntentTypeDef,
+    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
-    EnumerationValueTypeDef,
+    EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
-    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
-    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MessageTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SlotDefaultValueTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
-    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
+    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
+    GetExportResponseTypeDef,
+    GetImportResponseTypeDef,
+    StartMigrationResponseTypeDef,
+    EnumerationValueUnionTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    PromptOutputTypeDef,
     PromptTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
+    SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
+    PromptUnionTypeDef,
     CreateBotVersionResponseTypeDef,
-    FollowUpPromptTypeDef,
+    FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
-    PutBotRequestRequestTypeDef,
     PutBotResponseTypeDef,
+    FollowUpPromptTypeDef,
+    PutBotRequestRequestTypeDef,
+    StatementUnionTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
+    FollowUpPromptUnionTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
-    PutIntentRequestRequestTypeDef,
     PutIntentResponseTypeDef,
+    SlotUnionTypeDef,
+    PutIntentRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BotChannelAssociationTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lex-models-2.5.2/README.md` & `types-aiobotocore-lex-models-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-lex-models"></a>
 
 # types-aiobotocore-lex-models
 
 [![PyPI - types-aiobotocore-lex-models](https://img.shields.io/pypi/v/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [types-aiobotocore-lex-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/).
 
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
@@ -334,146 +334,158 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lex_models.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lex_models.type_defs import (
+    BlobTypeDef,
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     IntentTypeDef,
+    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
-    EnumerationValueTypeDef,
+    EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
-    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
-    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MessageTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SlotDefaultValueTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
-    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
+    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
+    GetExportResponseTypeDef,
+    GetImportResponseTypeDef,
+    StartMigrationResponseTypeDef,
+    EnumerationValueUnionTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    PromptOutputTypeDef,
     PromptTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
+    SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
+    PromptUnionTypeDef,
     CreateBotVersionResponseTypeDef,
-    FollowUpPromptTypeDef,
+    FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
-    PutBotRequestRequestTypeDef,
     PutBotResponseTypeDef,
+    FollowUpPromptTypeDef,
+    PutBotRequestRequestTypeDef,
+    StatementUnionTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
+    FollowUpPromptUnionTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
-    PutIntentRequestRequestTypeDef,
     PutIntentResponseTypeDef,
+    SlotUnionTypeDef,
+    PutIntentRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BotChannelAssociationTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lex-models-2.5.2/setup.py` & `types-aiobotocore-lex-models-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-models",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with"
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
-    keywords="aiobotocore lex-models type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore lex-models type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lex_models": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/"
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.py` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.pyi` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__main__.py` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LexModelBuildingService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.py` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("lex-models") as client:
         client: LexModelBuildingServiceClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ExportTypeType,
     LocaleType,
     MergeStrategyType,
     MigrationSortAttributeType,
@@ -43,22 +42,23 @@
     GetBuiltinSlotTypesPaginator,
     GetIntentsPaginator,
     GetIntentVersionsPaginator,
     GetSlotTypesPaginator,
     GetSlotTypeVersionsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnumerationValueTypeDef,
-    FollowUpPromptTypeDef,
+    EnumerationValueUnionTypeDef,
+    FollowUpPromptUnionTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
     GetBotsResponseTypeDef,
@@ -78,24 +78,24 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
-    PromptTypeDef,
+    PromptUnionTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
     SlotTypeConfigurationTypeDef,
-    SlotTypeDef,
+    SlotUnionTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
-    StatementTypeDef,
+    StatementUnionTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -524,16 +524,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: PromptTypeDef = ...,
-        abortStatement: StatementTypeDef = ...,
+        clarificationPrompt: PromptUnionTypeDef = ...,
+        abortStatement: StatementUnionTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -565,20 +565,20 @@
         """
 
     async def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[SlotTypeDef] = ...,
+        slots: Sequence[SlotUnionTypeDef] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: PromptTypeDef = ...,
-        rejectionStatement: StatementTypeDef = ...,
-        followUpPrompt: FollowUpPromptTypeDef = ...,
-        conclusionStatement: StatementTypeDef = ...,
+        confirmationPrompt: PromptUnionTypeDef = ...,
+        rejectionStatement: StatementUnionTypeDef = ...,
+        followUpPrompt: FollowUpPromptUnionTypeDef = ...,
+        conclusionStatement: StatementUnionTypeDef = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -592,15 +592,15 @@
         """
 
     async def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
+        enumerationValues: Sequence[EnumerationValueUnionTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
@@ -609,15 +609,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_slot_type)
         """
 
     async def start_import(
         self,
         *,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
+        payload: BlobTypeDef,
         resourceType: ResourceTypeType,
         mergeStrategy: MergeStrategyType,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts a job to import a resource to Amazon Lex.
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.pyi` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("lex-models") as client:
         client: LexModelBuildingServiceClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ExportTypeType,
     LocaleType,
     MergeStrategyType,
     MigrationSortAttributeType,
@@ -43,22 +42,23 @@
     GetBuiltinSlotTypesPaginator,
     GetIntentsPaginator,
     GetIntentVersionsPaginator,
     GetSlotTypesPaginator,
     GetSlotTypeVersionsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnumerationValueTypeDef,
-    FollowUpPromptTypeDef,
+    EnumerationValueUnionTypeDef,
+    FollowUpPromptUnionTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
     GetBotsResponseTypeDef,
@@ -78,24 +78,24 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
-    PromptTypeDef,
+    PromptUnionTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
     SlotTypeConfigurationTypeDef,
-    SlotTypeDef,
+    SlotUnionTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
-    StatementTypeDef,
+    StatementUnionTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -482,16 +482,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: PromptTypeDef = ...,
-        abortStatement: StatementTypeDef = ...,
+        clarificationPrompt: PromptUnionTypeDef = ...,
+        abortStatement: StatementUnionTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -521,20 +521,20 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_bot_alias)
         """
     async def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[SlotTypeDef] = ...,
+        slots: Sequence[SlotUnionTypeDef] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: PromptTypeDef = ...,
-        rejectionStatement: StatementTypeDef = ...,
-        followUpPrompt: FollowUpPromptTypeDef = ...,
-        conclusionStatement: StatementTypeDef = ...,
+        confirmationPrompt: PromptUnionTypeDef = ...,
+        rejectionStatement: StatementUnionTypeDef = ...,
+        followUpPrompt: FollowUpPromptUnionTypeDef = ...,
+        conclusionStatement: StatementUnionTypeDef = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -547,15 +547,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_intent)
         """
     async def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
+        enumerationValues: Sequence[EnumerationValueUnionTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
@@ -563,15 +563,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_slot_type)
         """
     async def start_import(
         self,
         *,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
+        payload: BlobTypeDef,
         resourceType: ResourceTypeType,
         mergeStrategy: MergeStrategyType,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts a job to import a resource to Amazon Lex.
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.py` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.pyi` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.py` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,183 +67,171 @@
     "GetBuiltinSlotTypesPaginator",
     "GetIntentVersionsPaginator",
     "GetIntentsPaginator",
     "GetSlotTypeVersionsPaginator",
     "GetSlotTypesPaginator",
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
 class GetBotAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotaliasespaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotaliasespaginator)
         """
 
-
 class GetBotChannelAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotchannelassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
-
 class GetBotVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotversionspaginator)
         """
 
-
 class GetBotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotspaginator)
         """
 
-
 class GetBuiltinIntentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinintentspaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
-
 class GetBuiltinSlotTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinslottypespaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
-
 class GetIntentVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentversionspaginator)
         """
 
-
 class GetIntentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentspaginator)
         """
 
-
 class GetSlotTypeVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypeversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSlotTypeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypeversionspaginator)
         """
 
-
 class GetSlotTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypespaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypespaginator)
         """
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.pyi` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,171 +67,183 @@
     "GetBuiltinSlotTypesPaginator",
     "GetIntentVersionsPaginator",
     "GetIntentsPaginator",
     "GetSlotTypeVersionsPaginator",
     "GetSlotTypesPaginator",
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
 class GetBotAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotaliasespaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotaliasespaginator)
         """
 
+
 class GetBotChannelAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotchannelassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
+
 class GetBotVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotversionspaginator)
         """
 
+
 class GetBotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotspaginator)
         """
 
+
 class GetBuiltinIntentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinintentspaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
+
 class GetBuiltinSlotTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinslottypespaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
+
 class GetIntentVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentversionspaginator)
         """
 
+
 class GetIntentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getintentspaginator)
         """
 
+
 class GetSlotTypeVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypeversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSlotTypeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypeversionspaginator)
         """
 
+
 class GetSlotTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypespaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getslottypespaginator)
         """
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.py` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-models service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_lex_models.type_defs import BotChannelAssociationTypeDef
+    from types_aiobotocore_lex_models.type_defs import BlobTypeDef
 
-    data: BotChannelAssociationTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -44,137 +44,149 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "BlobTypeDef",
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
     "IntentTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
-    "EnumerationValueTypeDef",
+    "EnumerationValueOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
-    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
-    "GetBotChannelAssociationResponseTypeDef",
-    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
-    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
-    "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBotsRequestRequestTypeDef",
     "GetBuiltinIntentRequestRequestTypeDef",
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinIntentsRequestRequestTypeDef",
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
-    "GetExportResponseTypeDef",
     "GetImportRequestRequestTypeDef",
-    "GetImportResponseTypeDef",
     "GetIntentRequestRequestTypeDef",
-    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     "GetIntentVersionsRequestRequestTypeDef",
     "IntentMetadataTypeDef",
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
     "GetIntentsRequestRequestTypeDef",
     "GetMigrationRequestRequestTypeDef",
     "MigrationAlertTypeDef",
     "GetMigrationsRequestRequestTypeDef",
     "MigrationSummaryTypeDef",
     "GetSlotTypeRequestRequestTypeDef",
-    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MessageTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
-    "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
+    "FulfillmentActivityTypeDef",
+    "ConversationLogsRequestTypeDef",
+    "ConversationLogsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
-    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
+    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
-    "FulfillmentActivityTypeDef",
-    "ConversationLogsRequestTypeDef",
-    "ConversationLogsResponseTypeDef",
+    "GetExportResponseTypeDef",
+    "GetImportResponseTypeDef",
+    "StartMigrationResponseTypeDef",
+    "EnumerationValueUnionTypeDef",
+    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "PromptOutputTypeDef",
     "PromptTypeDef",
+    "StatementOutputTypeDef",
     "StatementTypeDef",
+    "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
+    "PromptUnionTypeDef",
     "CreateBotVersionResponseTypeDef",
-    "FollowUpPromptTypeDef",
+    "FollowUpPromptOutputTypeDef",
     "GetBotResponseTypeDef",
-    "PutBotRequestRequestTypeDef",
     "PutBotResponseTypeDef",
+    "FollowUpPromptTypeDef",
+    "PutBotRequestRequestTypeDef",
+    "StatementUnionTypeDef",
+    "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
+    "FollowUpPromptUnionTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
-    "PutIntentRequestRequestTypeDef",
     "PutIntentResponseTypeDef",
+    "SlotUnionTypeDef",
+    "PutIntentRequestRequestTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
         "description": str,
         "botAlias": str,
         "botName": str,
@@ -246,21 +258,19 @@
     "_OptionalLogSettingsRequestTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class LogSettingsRequestTypeDef(
     _RequiredLogSettingsRequestTypeDef, _OptionalLogSettingsRequestTypeDef
 ):
     pass
 
-
 LogSettingsResponseTypeDef = TypedDict(
     "LogSettingsResponseTypeDef",
     {
         "logType": LogTypeType,
         "destination": DestinationType,
         "kmsKeyArn": str,
         "resourceArn": str,
@@ -279,51 +289,58 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-
 IntentTypeDef = TypedDict(
     "IntentTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
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
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntentVersionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateIntentVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateIntentVersionRequestRequestTypeDef(
     _RequiredCreateIntentVersionRequestRequestTypeDef,
     _OptionalCreateIntentVersionRequestRequestTypeDef,
 ):
     pass
 
-
 InputContextTypeDef = TypedDict(
     "InputContextTypeDef",
     {
         "name": str,
     },
 )
 
@@ -338,21 +355,19 @@
     "_OptionalKendraConfigurationTypeDef",
     {
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
@@ -368,41 +383,39 @@
     "_OptionalCreateSlotTypeVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredEnumerationValueTypeDef = TypedDict(
-    "_RequiredEnumerationValueTypeDef",
+_RequiredEnumerationValueOutputTypeDef = TypedDict(
+    "_RequiredEnumerationValueOutputTypeDef",
     {
         "value": str,
     },
 )
-_OptionalEnumerationValueTypeDef = TypedDict(
-    "_OptionalEnumerationValueTypeDef",
+_OptionalEnumerationValueOutputTypeDef = TypedDict(
+    "_OptionalEnumerationValueOutputTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
-
-class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+class EnumerationValueOutputTypeDef(
+    _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
+):
     pass
 
-
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -465,52 +478,49 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_RequiredEnumerationValueTypeDef = TypedDict(
+    "_RequiredEnumerationValueTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "value": str,
     },
 )
+_OptionalEnumerationValueTypeDef = TypedDict(
+    "_OptionalEnumerationValueTypeDef",
+    {
+        "synonyms": Sequence[str],
+    },
+    total=False,
+)
+
+class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+    pass
 
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
 
-_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "botName": str,
-    },
-)
-_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
-    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -519,70 +529,28 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
-
 class GetBotAliasesRequestRequestTypeDef(
     _RequiredGetBotAliasesRequestRequestTypeDef, _OptionalGetBotAliasesRequestRequestTypeDef
 ):
     pass
 
-
 GetBotChannelAssociationRequestRequestTypeDef = TypedDict(
     "GetBotChannelAssociationRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
 )
 
-GetBotChannelAssociationResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "botAlias": str,
-        "botName": str,
-        "createdDate": datetime,
-        "type": ChannelTypeType,
-        "botConfiguration": Dict[str, str],
-        "status": ChannelStatusType,
-        "failureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-    },
-)
-_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
-    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -592,52 +560,28 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
-
 class GetBotChannelAssociationsRequestRequestTypeDef(
     _RequiredGetBotChannelAssociationsRequestRequestTypeDef,
     _OptionalGetBotChannelAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 GetBotRequestRequestTypeDef = TypedDict(
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
 
-_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
-    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -645,30 +589,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
-
-GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBotsRequestRequestTypeDef = TypedDict(
     "GetBotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -678,45 +611,25 @@
 GetBuiltinIntentRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentRequestRequestTypeDef",
     {
         "signature": str,
     },
 )
 
-GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinIntentsRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentsRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinSlotTypesRequestRequestTypeDef = TypedDict(
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
@@ -730,79 +643,29 @@
         "name": str,
         "version": str,
         "resourceType": ResourceTypeType,
         "exportType": ExportTypeType,
     },
 )
 
-GetExportResponseTypeDef = TypedDict(
-    "GetExportResponseTypeDef",
-    {
-        "name": str,
-        "version": str,
-        "resourceType": ResourceTypeType,
-        "exportType": ExportTypeType,
-        "exportStatus": ExportStatusType,
-        "failureReason": str,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImportRequestRequestTypeDef = TypedDict(
     "GetImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-GetImportResponseTypeDef = TypedDict(
-    "GetImportResponseTypeDef",
-    {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIntentRequestRequestTypeDef = TypedDict(
     "GetIntentRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
-    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -810,42 +673,31 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetIntentVersionsRequestRequestTypeDef(
     _RequiredGetIntentVersionsRequestRequestTypeDef, _OptionalGetIntentVersionsRequestRequestTypeDef
 ):
     pass
 
-
 IntentMetadataTypeDef = TypedDict(
     "IntentMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetIntentsRequestRequestTypeDef = TypedDict(
     "GetIntentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -903,36 +755,14 @@
     "GetSlotTypeRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
-    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -940,43 +770,32 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetSlotTypeVersionsRequestRequestTypeDef(
     _RequiredGetSlotTypeVersionsRequestRequestTypeDef,
     _OptionalGetSlotTypeVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 SlotTypeMetadataTypeDef = TypedDict(
     "SlotTypeMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSlotTypesRequestRequestTypeDef = TypedDict(
     "GetSlotTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -1018,40 +837,17 @@
     "_OptionalMessageTypeDef",
     {
         "groupNumber": int,
     },
     total=False,
 )
 
-
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
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
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
@@ -1069,29 +865,14 @@
         "v1BotVersion": str,
         "v2BotName": str,
         "v2BotRole": str,
         "migrationStrategy": MigrationStrategyType,
     },
 )
 
-StartMigrationResponseTypeDef = TypedDict(
-    "StartMigrationResponseTypeDef",
-    {
-        "v1BotName": str,
-        "v1BotVersion": str,
-        "v1BotLocale": LocaleType,
-        "v2BotId": str,
-        "v2BotRole": str,
-        "migrationId": str,
-        "migrationStrategy": MigrationStrategyType,
-        "migrationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1104,122 +885,337 @@
         "distinctUsers": int,
         "firstUtteredDate": datetime,
         "lastUtteredDate": datetime,
     },
     total=False,
 )
 
+_RequiredFulfillmentActivityTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityTypeDef",
+    {
+        "type": FulfillmentActivityTypeType,
+    },
+)
+_OptionalFulfillmentActivityTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityTypeDef",
+    {
+        "codeHook": CodeHookTypeDef,
+    },
+    total=False,
+)
+
+class FulfillmentActivityTypeDef(
+    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+):
+    pass
+
+ConversationLogsRequestTypeDef = TypedDict(
+    "ConversationLogsRequestTypeDef",
+    {
+        "logSettings": Sequence[LogSettingsRequestTypeDef],
+        "iamRoleArn": str,
+    },
+)
+
+ConversationLogsResponseTypeDef = TypedDict(
+    "ConversationLogsResponseTypeDef",
+    {
+        "logSettings": List[LogSettingsResponseTypeDef],
+        "iamRoleArn": str,
+    },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBotChannelAssociationResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "botAlias": str,
+        "botName": str,
+        "createdDate": datetime,
+        "type": ChannelTypeType,
+        "botConfiguration": Dict[str, str],
+        "status": ChannelStatusType,
+        "failureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetBotChannelAssociationsResponseTypeDef = TypedDict(
     "GetBotChannelAssociationsResponseTypeDef",
     {
         "botChannelAssociations": List[BotChannelAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotVersionsResponseTypeDef = TypedDict(
     "GetBotVersionsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotsResponseTypeDef = TypedDict(
     "GetBotsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetBuiltinIntentsResponseTypeDef = TypedDict(
-    "GetBuiltinIntentsResponseTypeDef",
-    {
-        "intents": List[BuiltinIntentMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBuiltinIntentResponseTypeDef = TypedDict(
     "GetBuiltinIntentResponseTypeDef",
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
         "slots": List[BuiltinIntentSlotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBuiltinIntentsResponseTypeDef = TypedDict(
+    "GetBuiltinIntentsResponseTypeDef",
+    {
+        "intents": List[BuiltinIntentMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBuiltinSlotTypesResponseTypeDef = TypedDict(
     "GetBuiltinSlotTypesResponseTypeDef",
     {
         "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFulfillmentActivityTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityTypeDef",
+GetExportResponseTypeDef = TypedDict(
+    "GetExportResponseTypeDef",
     {
-        "type": FulfillmentActivityTypeType,
+        "name": str,
+        "version": str,
+        "resourceType": ResourceTypeType,
+        "exportType": ExportTypeType,
+        "exportStatus": ExportStatusType,
+        "failureReason": str,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFulfillmentActivityTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityTypeDef",
+
+GetImportResponseTypeDef = TypedDict(
+    "GetImportResponseTypeDef",
     {
-        "codeHook": CodeHookTypeDef,
+        "name": str,
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMigrationResponseTypeDef = TypedDict(
+    "StartMigrationResponseTypeDef",
+    {
+        "v1BotName": str,
+        "v1BotVersion": str,
+        "v1BotLocale": LocaleType,
+        "v2BotId": str,
+        "v2BotRole": str,
+        "migrationId": str,
+        "migrationStrategy": MigrationStrategyType,
+        "migrationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnumerationValueUnionTypeDef = Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
+_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    {
+        "botName": str,
+    },
+)
+_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
+    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+):
+    pass
 
-class FulfillmentActivityTypeDef(
-    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+    },
+)
+_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
+    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
 ):
     pass
 
+_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ConversationLogsRequestTypeDef = TypedDict(
-    "ConversationLogsRequestTypeDef",
+class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
+    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+):
+    pass
+
+GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
+    "GetBotsRequestGetBotsPaginateTypeDef",
     {
-        "logSettings": Sequence[LogSettingsRequestTypeDef],
-        "iamRoleArn": str,
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ConversationLogsResponseTypeDef = TypedDict(
-    "ConversationLogsResponseTypeDef",
+GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     {
-        "logSettings": List[LogSettingsResponseTypeDef],
-        "iamRoleArn": str,
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
+    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+):
+    pass
+
+GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
+    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+):
+    pass
+
+GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetIntentVersionsResponseTypeDef = TypedDict(
     "GetIntentVersionsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentsResponseTypeDef = TypedDict(
     "GetIntentsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationResponseTypeDef = TypedDict(
     "GetMigrationResponseTypeDef",
     {
         "migrationId": str,
@@ -1228,141 +1224,177 @@
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationStatus": MigrationStatusType,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "alerts": List[MigrationAlertTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationsResponseTypeDef = TypedDict(
     "GetMigrationsResponseTypeDef",
     {
         "migrationSummaries": List[MigrationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeVersionsResponseTypeDef = TypedDict(
     "GetSlotTypeVersionsResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypesResponseTypeDef = TypedDict(
     "GetSlotTypesResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
     },
 )
 _OptionalStartImportRequestRequestTypeDef = TypedDict(
     "_OptionalStartImportRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
-
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
         "importId": str,
         "importStatus": ImportStatusType,
         "tags": List[TagTypeDef],
         "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredPromptOutputTypeDef = TypedDict(
+    "_RequiredPromptOutputTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+        "maxAttempts": int,
+    },
+)
+_OptionalPromptOutputTypeDef = TypedDict(
+    "_OptionalPromptOutputTypeDef",
+    {
+        "responseCard": str,
+    },
+    total=False,
+)
+
+class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
+    pass
+
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptTypeDef = TypedDict(
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
+_RequiredStatementOutputTypeDef = TypedDict(
+    "_RequiredStatementOutputTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+    },
+)
+_OptionalStatementOutputTypeDef = TypedDict(
+    "_OptionalStatementOutputTypeDef",
+    {
+        "responseCard": str,
+    },
+    total=False,
+)
+
+class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
+    pass
 
 _RequiredStatementTypeDef = TypedDict(
     "_RequiredStatementTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
     },
 )
 _OptionalStatementTypeDef = TypedDict(
     "_OptionalStatementTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
 class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
+SlotDefaultValueSpecOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueTypeDef],
+    },
+)
 
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
+        "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
@@ -1394,21 +1426,19 @@
         "checksum": str,
         "conversationLogs": ConversationLogsRequestTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutBotAliasRequestRequestTypeDef(
     _RequiredPutBotAliasRequestRequestTypeDef, _OptionalPutBotAliasRequestRequestTypeDef
 ):
     pass
 
-
 BotAliasMetadataTypeDef = TypedDict(
     "BotAliasMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
@@ -1427,15 +1457,15 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBotAliasResponseTypeDef = TypedDict(
     "PutBotAliasResponseTypeDef",
     {
         "name": str,
@@ -1443,72 +1473,108 @@
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PromptUnionTypeDef = Union[PromptTypeDef, PromptOutputTypeDef]
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptTypeDef = TypedDict(
-    "FollowUpPromptTypeDef",
+FollowUpPromptOutputTypeDef = TypedDict(
+    "FollowUpPromptOutputTypeDef",
     {
-        "prompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
+        "prompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutBotResponseTypeDef = TypedDict(
+    "PutBotResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "intents": List[IntentTypeDef],
+        "enableModelImprovements": bool,
+        "nluIntentConfidenceThreshold": float,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
+        "status": StatusType,
+        "failureReason": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "idleSessionTTLInSeconds": int,
+        "voiceId": str,
+        "checksum": str,
+        "version": str,
+        "locale": LocaleType,
+        "childDirected": bool,
+        "createVersion": bool,
+        "detectSentiment": bool,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FollowUpPromptTypeDef = TypedDict(
+    "FollowUpPromptTypeDef",
+    {
+        "prompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
     },
 )
 
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
@@ -1532,48 +1598,46 @@
         "detectSentiment": bool,
         "createVersion": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
-
-PutBotResponseTypeDef = TypedDict(
-    "PutBotResponseTypeDef",
+StatementUnionTypeDef = Union[StatementTypeDef, StatementOutputTypeDef]
+_RequiredSlotOutputTypeDef = TypedDict(
+    "_RequiredSlotOutputTypeDef",
     {
         "name": str,
+        "slotConstraint": SlotConstraintType,
+    },
+)
+_OptionalSlotOutputTypeDef = TypedDict(
+    "_OptionalSlotOutputTypeDef",
+    {
         "description": str,
-        "intents": List[IntentTypeDef],
-        "enableModelImprovements": bool,
-        "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
-        "status": StatusType,
-        "failureReason": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "idleSessionTTLInSeconds": int,
-        "voiceId": str,
-        "checksum": str,
-        "version": str,
-        "locale": LocaleType,
-        "childDirected": bool,
-        "createVersion": bool,
-        "detectSentiment": bool,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotType": str,
+        "slotTypeVersion": str,
+        "valueElicitationPrompt": PromptOutputTypeDef,
+        "priority": int,
+        "sampleUtterances": List[str],
+        "responseCard": str,
+        "obfuscationSetting": ObfuscationSettingType,
+        "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
     },
+    total=False,
 )
 
+class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
+    pass
+
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1581,185 +1645,209 @@
     "_OptionalSlotTypeDef",
     {
         "description": str,
         "slotType": str,
         "slotTypeVersion": str,
         "valueElicitationPrompt": PromptTypeDef,
         "priority": int,
-        "sampleUtterances": List[str],
+        "sampleUtterances": Sequence[str],
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
-
 class SlotTypeDef(_RequiredSlotTypeDef, _OptionalSlotTypeDef):
     pass
 
-
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[EnumerationValueTypeDef],
+        "enumerationValues": Sequence[EnumerationValueUnionTypeDef],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class PutSlotTypeRequestRequestTypeDef(
     _RequiredPutSlotTypeRequestRequestTypeDef, _OptionalPutSlotTypeRequestRequestTypeDef
 ):
     pass
 
-
 PutSlotTypeResponseTypeDef = TypedDict(
     "PutSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotAliasesResponseTypeDef = TypedDict(
     "GetBotAliasesResponseTypeDef",
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FollowUpPromptUnionTypeDef = Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef]
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutIntentResponseTypeDef = TypedDict(
+    "PutIntentResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "slots": List[SlotOutputTypeDef],
+        "sampleUtterances": List[str],
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "parentIntentSignature": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "createVersion": bool,
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SlotUnionTypeDef = Union[SlotTypeDef, SlotOutputTypeDef]
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[SlotTypeDef],
+        "slots": Sequence[SlotUnionTypeDef],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
@@ -1769,39 +1857,11 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
     },
     total=False,
 )
 
-
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
-
-
-PutIntentResponseTypeDef = TypedDict(
-    "PutIntentResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "slots": List[SlotTypeDef],
-        "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
-        "parentIntentSignature": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "createVersion": bool,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.pyi` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-models service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_lex_models.type_defs import BotChannelAssociationTypeDef
+    from types_aiobotocore_lex_models.type_defs import BlobTypeDef
 
-    data: BotChannelAssociationTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -44,136 +44,150 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "BlobTypeDef",
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
     "IntentTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
-    "EnumerationValueTypeDef",
+    "EnumerationValueOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
-    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
-    "GetBotChannelAssociationResponseTypeDef",
-    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
-    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
-    "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBotsRequestRequestTypeDef",
     "GetBuiltinIntentRequestRequestTypeDef",
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinIntentsRequestRequestTypeDef",
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
-    "GetExportResponseTypeDef",
     "GetImportRequestRequestTypeDef",
-    "GetImportResponseTypeDef",
     "GetIntentRequestRequestTypeDef",
-    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     "GetIntentVersionsRequestRequestTypeDef",
     "IntentMetadataTypeDef",
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
     "GetIntentsRequestRequestTypeDef",
     "GetMigrationRequestRequestTypeDef",
     "MigrationAlertTypeDef",
     "GetMigrationsRequestRequestTypeDef",
     "MigrationSummaryTypeDef",
     "GetSlotTypeRequestRequestTypeDef",
-    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MessageTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
-    "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
+    "FulfillmentActivityTypeDef",
+    "ConversationLogsRequestTypeDef",
+    "ConversationLogsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
-    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
+    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
-    "FulfillmentActivityTypeDef",
-    "ConversationLogsRequestTypeDef",
-    "ConversationLogsResponseTypeDef",
+    "GetExportResponseTypeDef",
+    "GetImportResponseTypeDef",
+    "StartMigrationResponseTypeDef",
+    "EnumerationValueUnionTypeDef",
+    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "PromptOutputTypeDef",
     "PromptTypeDef",
+    "StatementOutputTypeDef",
     "StatementTypeDef",
+    "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
+    "PromptUnionTypeDef",
     "CreateBotVersionResponseTypeDef",
-    "FollowUpPromptTypeDef",
+    "FollowUpPromptOutputTypeDef",
     "GetBotResponseTypeDef",
-    "PutBotRequestRequestTypeDef",
     "PutBotResponseTypeDef",
+    "FollowUpPromptTypeDef",
+    "PutBotRequestRequestTypeDef",
+    "StatementUnionTypeDef",
+    "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
+    "FollowUpPromptUnionTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
-    "PutIntentRequestRequestTypeDef",
     "PutIntentResponseTypeDef",
+    "SlotUnionTypeDef",
+    "PutIntentRequestRequestTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
         "description": str,
         "botAlias": str,
         "botName": str,
@@ -245,19 +259,21 @@
     "_OptionalLogSettingsRequestTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class LogSettingsRequestTypeDef(
     _RequiredLogSettingsRequestTypeDef, _OptionalLogSettingsRequestTypeDef
 ):
     pass
 
+
 LogSettingsResponseTypeDef = TypedDict(
     "LogSettingsResponseTypeDef",
     {
         "logType": LogTypeType,
         "destination": DestinationType,
         "kmsKeyArn": str,
         "resourceArn": str,
@@ -276,47 +292,62 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
+
 IntentTypeDef = TypedDict(
     "IntentTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
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
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntentVersionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateIntentVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateIntentVersionRequestRequestTypeDef(
     _RequiredCreateIntentVersionRequestRequestTypeDef,
     _OptionalCreateIntentVersionRequestRequestTypeDef,
 ):
     pass
 
+
 InputContextTypeDef = TypedDict(
     "InputContextTypeDef",
     {
         "name": str,
     },
 )
 
@@ -331,19 +362,21 @@
     "_OptionalKendraConfigurationTypeDef",
     {
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
@@ -359,37 +392,43 @@
     "_OptionalCreateSlotTypeVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEnumerationValueTypeDef = TypedDict(
-    "_RequiredEnumerationValueTypeDef",
+
+_RequiredEnumerationValueOutputTypeDef = TypedDict(
+    "_RequiredEnumerationValueOutputTypeDef",
     {
         "value": str,
     },
 )
-_OptionalEnumerationValueTypeDef = TypedDict(
-    "_OptionalEnumerationValueTypeDef",
+_OptionalEnumerationValueOutputTypeDef = TypedDict(
+    "_OptionalEnumerationValueOutputTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
-class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+
+class EnumerationValueOutputTypeDef(
+    _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
+):
     pass
 
+
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -452,50 +491,51 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_RequiredEnumerationValueTypeDef = TypedDict(
+    "_RequiredEnumerationValueTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "value": str,
+    },
+)
+_OptionalEnumerationValueTypeDef = TypedDict(
+    "_OptionalEnumerationValueTypeDef",
+    {
+        "synonyms": Sequence[str],
     },
+    total=False,
 )
 
+
+class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+    pass
+
+
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
 
-_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "botName": str,
-    },
-)
-_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
-    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -504,66 +544,30 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
+
 class GetBotAliasesRequestRequestTypeDef(
     _RequiredGetBotAliasesRequestRequestTypeDef, _OptionalGetBotAliasesRequestRequestTypeDef
 ):
     pass
 
+
 GetBotChannelAssociationRequestRequestTypeDef = TypedDict(
     "GetBotChannelAssociationRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
 )
 
-GetBotChannelAssociationResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "botAlias": str,
-        "botName": str,
-        "createdDate": datetime,
-        "type": ChannelTypeType,
-        "botConfiguration": Dict[str, str],
-        "status": ChannelStatusType,
-        "failureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-    },
-)
-_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
-    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -573,48 +577,30 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
+
 class GetBotChannelAssociationsRequestRequestTypeDef(
     _RequiredGetBotChannelAssociationsRequestRequestTypeDef,
     _OptionalGetBotChannelAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 GetBotRequestRequestTypeDef = TypedDict(
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
 
-_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
-    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -622,27 +608,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
-GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 GetBotsRequestRequestTypeDef = TypedDict(
     "GetBotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
@@ -653,45 +632,25 @@
 GetBuiltinIntentRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentRequestRequestTypeDef",
     {
         "signature": str,
     },
 )
 
-GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinIntentsRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentsRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinSlotTypesRequestRequestTypeDef = TypedDict(
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
@@ -705,77 +664,29 @@
         "name": str,
         "version": str,
         "resourceType": ResourceTypeType,
         "exportType": ExportTypeType,
     },
 )
 
-GetExportResponseTypeDef = TypedDict(
-    "GetExportResponseTypeDef",
-    {
-        "name": str,
-        "version": str,
-        "resourceType": ResourceTypeType,
-        "exportType": ExportTypeType,
-        "exportStatus": ExportStatusType,
-        "failureReason": str,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImportRequestRequestTypeDef = TypedDict(
     "GetImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-GetImportResponseTypeDef = TypedDict(
-    "GetImportResponseTypeDef",
-    {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIntentRequestRequestTypeDef = TypedDict(
     "GetIntentRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
-    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -783,40 +694,33 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetIntentVersionsRequestRequestTypeDef(
     _RequiredGetIntentVersionsRequestRequestTypeDef, _OptionalGetIntentVersionsRequestRequestTypeDef
 ):
     pass
 
+
 IntentMetadataTypeDef = TypedDict(
     "IntentMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetIntentsRequestRequestTypeDef = TypedDict(
     "GetIntentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -874,34 +778,14 @@
     "GetSlotTypeRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
-    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -909,41 +793,34 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetSlotTypeVersionsRequestRequestTypeDef(
     _RequiredGetSlotTypeVersionsRequestRequestTypeDef,
     _OptionalGetSlotTypeVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 SlotTypeMetadataTypeDef = TypedDict(
     "SlotTypeMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSlotTypesRequestRequestTypeDef = TypedDict(
     "GetSlotTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -985,37 +862,18 @@
     "_OptionalMessageTypeDef",
     {
         "groupNumber": int,
     },
     total=False,
 )
 
+
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
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
 
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
@@ -1034,29 +892,14 @@
         "v1BotVersion": str,
         "v2BotName": str,
         "v2BotRole": str,
         "migrationStrategy": MigrationStrategyType,
     },
 )
 
-StartMigrationResponseTypeDef = TypedDict(
-    "StartMigrationResponseTypeDef",
-    {
-        "v1BotName": str,
-        "v1BotVersion": str,
-        "v1BotLocale": LocaleType,
-        "v2BotId": str,
-        "v2BotRole": str,
-        "migrationId": str,
-        "migrationStrategy": MigrationStrategyType,
-        "migrationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1069,120 +912,349 @@
         "distinctUsers": int,
         "firstUtteredDate": datetime,
         "lastUtteredDate": datetime,
     },
     total=False,
 )
 
+_RequiredFulfillmentActivityTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityTypeDef",
+    {
+        "type": FulfillmentActivityTypeType,
+    },
+)
+_OptionalFulfillmentActivityTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityTypeDef",
+    {
+        "codeHook": CodeHookTypeDef,
+    },
+    total=False,
+)
+
+
+class FulfillmentActivityTypeDef(
+    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+):
+    pass
+
+
+ConversationLogsRequestTypeDef = TypedDict(
+    "ConversationLogsRequestTypeDef",
+    {
+        "logSettings": Sequence[LogSettingsRequestTypeDef],
+        "iamRoleArn": str,
+    },
+)
+
+ConversationLogsResponseTypeDef = TypedDict(
+    "ConversationLogsResponseTypeDef",
+    {
+        "logSettings": List[LogSettingsResponseTypeDef],
+        "iamRoleArn": str,
+    },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBotChannelAssociationResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "botAlias": str,
+        "botName": str,
+        "createdDate": datetime,
+        "type": ChannelTypeType,
+        "botConfiguration": Dict[str, str],
+        "status": ChannelStatusType,
+        "failureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetBotChannelAssociationsResponseTypeDef = TypedDict(
     "GetBotChannelAssociationsResponseTypeDef",
     {
         "botChannelAssociations": List[BotChannelAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotVersionsResponseTypeDef = TypedDict(
     "GetBotVersionsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotsResponseTypeDef = TypedDict(
     "GetBotsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetBuiltinIntentsResponseTypeDef = TypedDict(
-    "GetBuiltinIntentsResponseTypeDef",
-    {
-        "intents": List[BuiltinIntentMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBuiltinIntentResponseTypeDef = TypedDict(
     "GetBuiltinIntentResponseTypeDef",
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
         "slots": List[BuiltinIntentSlotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBuiltinIntentsResponseTypeDef = TypedDict(
+    "GetBuiltinIntentsResponseTypeDef",
+    {
+        "intents": List[BuiltinIntentMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBuiltinSlotTypesResponseTypeDef = TypedDict(
     "GetBuiltinSlotTypesResponseTypeDef",
     {
         "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFulfillmentActivityTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityTypeDef",
+GetExportResponseTypeDef = TypedDict(
+    "GetExportResponseTypeDef",
     {
-        "type": FulfillmentActivityTypeType,
+        "name": str,
+        "version": str,
+        "resourceType": ResourceTypeType,
+        "exportType": ExportTypeType,
+        "exportStatus": ExportStatusType,
+        "failureReason": str,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFulfillmentActivityTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityTypeDef",
+
+GetImportResponseTypeDef = TypedDict(
+    "GetImportResponseTypeDef",
     {
-        "codeHook": CodeHookTypeDef,
+        "name": str,
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMigrationResponseTypeDef = TypedDict(
+    "StartMigrationResponseTypeDef",
+    {
+        "v1BotName": str,
+        "v1BotVersion": str,
+        "v1BotLocale": LocaleType,
+        "v2BotId": str,
+        "v2BotRole": str,
+        "migrationId": str,
+        "migrationStrategy": MigrationStrategyType,
+        "migrationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnumerationValueUnionTypeDef = Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
+_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    {
+        "botName": str,
+    },
+)
+_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class FulfillmentActivityTypeDef(
-    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+
+class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
+    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
 ):
     pass
 
-ConversationLogsRequestTypeDef = TypedDict(
-    "ConversationLogsRequestTypeDef",
+
+_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     {
-        "logSettings": Sequence[LogSettingsRequestTypeDef],
-        "iamRoleArn": str,
+        "botName": str,
+        "botAlias": str,
+    },
+)
+_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ConversationLogsResponseTypeDef = TypedDict(
-    "ConversationLogsResponseTypeDef",
+
+class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
+    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     {
-        "logSettings": List[LogSettingsResponseTypeDef],
-        "iamRoleArn": str,
+        "name": str,
+    },
+)
+_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
+    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+):
+    pass
+
+
+GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
+    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+):
+    pass
+
+
+GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
+    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+):
+    pass
+
+
+GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetIntentVersionsResponseTypeDef = TypedDict(
     "GetIntentVersionsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentsResponseTypeDef = TypedDict(
     "GetIntentsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationResponseTypeDef = TypedDict(
     "GetMigrationResponseTypeDef",
     {
         "migrationId": str,
@@ -1191,135 +1263,187 @@
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationStatus": MigrationStatusType,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "alerts": List[MigrationAlertTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationsResponseTypeDef = TypedDict(
     "GetMigrationsResponseTypeDef",
     {
         "migrationSummaries": List[MigrationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeVersionsResponseTypeDef = TypedDict(
     "GetSlotTypeVersionsResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypesResponseTypeDef = TypedDict(
     "GetSlotTypesResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
     },
 )
 _OptionalStartImportRequestRequestTypeDef = TypedDict(
     "_OptionalStartImportRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
+
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
         "importId": str,
         "importStatus": ImportStatusType,
         "tags": List[TagTypeDef],
         "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredPromptOutputTypeDef = TypedDict(
+    "_RequiredPromptOutputTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+        "maxAttempts": int,
+    },
+)
+_OptionalPromptOutputTypeDef = TypedDict(
+    "_OptionalPromptOutputTypeDef",
+    {
+        "responseCard": str,
+    },
+    total=False,
+)
+
+
+class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
+    pass
+
+
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptTypeDef = TypedDict(
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
+
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
+
+_RequiredStatementOutputTypeDef = TypedDict(
+    "_RequiredStatementOutputTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+    },
+)
+_OptionalStatementOutputTypeDef = TypedDict(
+    "_OptionalStatementOutputTypeDef",
+    {
+        "responseCard": str,
+    },
+    total=False,
+)
+
+
+class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
+    pass
+
+
 _RequiredStatementTypeDef = TypedDict(
     "_RequiredStatementTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
     },
 )
 _OptionalStatementTypeDef = TypedDict(
     "_OptionalStatementTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
+
 class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
+
+SlotDefaultValueSpecOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueTypeDef],
+    },
+)
+
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
+        "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
@@ -1351,19 +1475,21 @@
         "checksum": str,
         "conversationLogs": ConversationLogsRequestTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutBotAliasRequestRequestTypeDef(
     _RequiredPutBotAliasRequestRequestTypeDef, _OptionalPutBotAliasRequestRequestTypeDef
 ):
     pass
 
+
 BotAliasMetadataTypeDef = TypedDict(
     "BotAliasMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
@@ -1382,15 +1508,15 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBotAliasResponseTypeDef = TypedDict(
     "PutBotAliasResponseTypeDef",
     {
         "name": str,
@@ -1398,72 +1524,108 @@
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PromptUnionTypeDef = Union[PromptTypeDef, PromptOutputTypeDef]
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptTypeDef = TypedDict(
-    "FollowUpPromptTypeDef",
+FollowUpPromptOutputTypeDef = TypedDict(
+    "FollowUpPromptOutputTypeDef",
     {
-        "prompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
+        "prompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutBotResponseTypeDef = TypedDict(
+    "PutBotResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "intents": List[IntentTypeDef],
+        "enableModelImprovements": bool,
+        "nluIntentConfidenceThreshold": float,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
+        "status": StatusType,
+        "failureReason": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "idleSessionTTLInSeconds": int,
+        "voiceId": str,
+        "checksum": str,
+        "version": str,
+        "locale": LocaleType,
+        "childDirected": bool,
+        "createVersion": bool,
+        "detectSentiment": bool,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FollowUpPromptTypeDef = TypedDict(
+    "FollowUpPromptTypeDef",
+    {
+        "prompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
     },
 )
 
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
@@ -1487,46 +1649,50 @@
         "detectSentiment": bool,
         "createVersion": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
-PutBotResponseTypeDef = TypedDict(
-    "PutBotResponseTypeDef",
+
+StatementUnionTypeDef = Union[StatementTypeDef, StatementOutputTypeDef]
+_RequiredSlotOutputTypeDef = TypedDict(
+    "_RequiredSlotOutputTypeDef",
     {
         "name": str,
+        "slotConstraint": SlotConstraintType,
+    },
+)
+_OptionalSlotOutputTypeDef = TypedDict(
+    "_OptionalSlotOutputTypeDef",
+    {
         "description": str,
-        "intents": List[IntentTypeDef],
-        "enableModelImprovements": bool,
-        "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
-        "status": StatusType,
-        "failureReason": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "idleSessionTTLInSeconds": int,
-        "voiceId": str,
-        "checksum": str,
-        "version": str,
-        "locale": LocaleType,
-        "childDirected": bool,
-        "createVersion": bool,
-        "detectSentiment": bool,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotType": str,
+        "slotTypeVersion": str,
+        "valueElicitationPrompt": PromptOutputTypeDef,
+        "priority": int,
+        "sampleUtterances": List[str],
+        "responseCard": str,
+        "obfuscationSetting": ObfuscationSettingType,
+        "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
     },
+    total=False,
 )
 
+
+class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
+    pass
+
+
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1534,181 +1700,213 @@
     "_OptionalSlotTypeDef",
     {
         "description": str,
         "slotType": str,
         "slotTypeVersion": str,
         "valueElicitationPrompt": PromptTypeDef,
         "priority": int,
-        "sampleUtterances": List[str],
+        "sampleUtterances": Sequence[str],
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
+
 class SlotTypeDef(_RequiredSlotTypeDef, _OptionalSlotTypeDef):
     pass
 
+
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[EnumerationValueTypeDef],
+        "enumerationValues": Sequence[EnumerationValueUnionTypeDef],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class PutSlotTypeRequestRequestTypeDef(
     _RequiredPutSlotTypeRequestRequestTypeDef, _OptionalPutSlotTypeRequestRequestTypeDef
 ):
     pass
 
+
 PutSlotTypeResponseTypeDef = TypedDict(
     "PutSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotAliasesResponseTypeDef = TypedDict(
     "GetBotAliasesResponseTypeDef",
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FollowUpPromptUnionTypeDef = Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef]
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "parentIntentSignature": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutIntentResponseTypeDef = TypedDict(
+    "PutIntentResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "slots": List[SlotOutputTypeDef],
+        "sampleUtterances": List[str],
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
+        "createVersion": bool,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SlotUnionTypeDef = Union[SlotTypeDef, SlotOutputTypeDef]
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[SlotTypeDef],
+        "slots": Sequence[SlotUnionTypeDef],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
@@ -1718,37 +1916,12 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
     },
     total=False,
 )
 
+
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
-
-PutIntentResponseTypeDef = TypedDict(
-    "PutIntentResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "slots": List[SlotTypeDef],
-        "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
-        "parentIntentSignature": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "createVersion": bool,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/PKG-INFO` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lex-models type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lex-models type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lex-models"></a>
 
 # types-aiobotocore-lex-models
 
 [![PyPI - types-aiobotocore-lex-models](https://img.shields.io/pypi/v/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [types-aiobotocore-lex-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/).
 
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
@@ -367,146 +366,158 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lex_models.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lex_models.type_defs import (
+    BlobTypeDef,
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     IntentTypeDef,
+    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
-    EnumerationValueTypeDef,
+    EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
-    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
-    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MessageTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SlotDefaultValueTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
-    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
+    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
+    GetExportResponseTypeDef,
+    GetImportResponseTypeDef,
+    StartMigrationResponseTypeDef,
+    EnumerationValueUnionTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    PromptOutputTypeDef,
     PromptTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
+    SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
+    PromptUnionTypeDef,
     CreateBotVersionResponseTypeDef,
-    FollowUpPromptTypeDef,
+    FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
-    PutBotRequestRequestTypeDef,
     PutBotResponseTypeDef,
+    FollowUpPromptTypeDef,
+    PutBotRequestRequestTypeDef,
+    StatementUnionTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
+    FollowUpPromptUnionTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
-    PutIntentRequestRequestTypeDef,
     PutIntentResponseTypeDef,
+    SlotUnionTypeDef,
+    PutIntentRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BotChannelAssociationTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/SOURCES.txt` & `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


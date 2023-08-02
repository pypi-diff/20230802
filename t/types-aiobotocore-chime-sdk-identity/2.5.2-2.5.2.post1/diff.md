# Comparing `tmp/types-aiobotocore-chime-sdk-identity-2.5.2.tar.gz` & `tmp/types-aiobotocore-chime-sdk-identity-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-identity-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-identity-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.tar` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.149780 types-aiobotocore-chime-sdk-identity-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-08 01:43:19.145780 types-aiobotocore-chime-sdk-identity-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:19.149780 types-aiobotocore-chime-sdk-identity-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.141780 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25396 2023-07-08 01:26:38.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25367 2023-07-08 01:26:38.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:37.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.145780 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 01:43:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25346 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25317 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/LICENSE` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/PKG-INFO` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-identity
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-identity type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-identity type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-identity"></a>
 
 # types-aiobotocore-chime-sdk-identity
 
 [![PyPI - types-aiobotocore-chime-sdk-identity](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-identity?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-identity)](https://pepy.tech/project/types-aiobotocore-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
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
@@ -288,80 +287,80 @@
 )
 
 
 def check_value(value: AllowMessagesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_identity.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_identity.type_defs import (
     IdentityTypeDef,
     AppInstanceBotSummaryTypeDef,
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceBotResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAppInstanceBotsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
     PutAppInstanceUserExpirationSettingsResponseTypeDef,
+    RegisterAppInstanceUserEndpointResponseTypeDef,
+    UpdateAppInstanceBotResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserEndpointResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
@@ -375,15 +374,15 @@
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
     UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityTypeDef:
+def get_value() -> IdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/README.md` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-chime-sdk-identity"></a>
 
 # types-aiobotocore-chime-sdk-identity
 
 [![PyPI - types-aiobotocore-chime-sdk-identity](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-identity?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-identity)](https://pepy.tech/project/types-aiobotocore-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
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
@@ -255,80 +255,80 @@
 )
 
 
 def check_value(value: AllowMessagesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_identity.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_identity.type_defs import (
     IdentityTypeDef,
     AppInstanceBotSummaryTypeDef,
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceBotResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAppInstanceBotsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
     PutAppInstanceUserExpirationSettingsResponseTypeDef,
+    RegisterAppInstanceUserEndpointResponseTypeDef,
+    UpdateAppInstanceBotResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserEndpointResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
@@ -342,15 +342,15 @@
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
     UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityTypeDef:
+def get_value() -> IdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/setup.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-identity",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_chime_sdk_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore chime-sdk-identity type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore chime-sdk-identity type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_identity": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/"
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/__init__.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/__init__.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/__main__.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/client.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/client.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/literals.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/literals.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/type_defs.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_identity.type_defs import IdentityTypeDef
 
-    data: IdentityTypeDef = {...}
+    data: IdentityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -41,61 +41,61 @@
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
     "EndpointAttributesTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateAppInstanceBotResponseTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceBotRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeregisterAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceAdminRequestRequestTypeDef",
     "DescribeAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceRequestRequestTypeDef",
     "DescribeAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceUserRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "InvokedByTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceBotsRequestRequestTypeDef",
     "ListAppInstanceUserEndpointsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppInstanceBotResponseTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserEndpointRequestRequestTypeDef",
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "ListAppInstanceBotsResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
     "AppInstanceUserEndpointSummaryTypeDef",
     "AppInstanceUserEndpointTypeDef",
     "RegisterAppInstanceUserEndpointRequestRequestTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
     "AppInstanceUserTypeDef",
     "PutAppInstanceUserExpirationSettingsRequestRequestTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateAppInstanceBotResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAppInstanceBotsResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    "UpdateAppInstanceBotResponseTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "LexConfigurationTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
@@ -223,43 +223,30 @@
     "CreateAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
         "AppInstanceArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-CreateAppInstanceBotResponseTypeDef = TypedDict(
-    "CreateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
 DeleteAppInstanceAdminRequestRequestTypeDef = TypedDict(
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
@@ -329,21 +316,14 @@
 DescribeAppInstanceUserRequestRequestTypeDef = TypedDict(
     "DescribeAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
@@ -459,67 +439,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAppInstanceBotResponseTypeDef = TypedDict(
-    "UpdateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAppInstanceRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
     },
 )
@@ -536,40 +480,23 @@
 class UpdateAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -580,58 +507,22 @@
         "Admin": IdentityTypeDef,
         "AppInstanceArn": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-CreateAppInstanceAdminResponseTypeDef = TypedDict(
-    "CreateAppInstanceAdminResponseTypeDef",
-    {
-        "AppInstanceAdmin": IdentityTypeDef,
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAppInstanceBotsResponseTypeDef = TypedDict(
-    "ListAppInstanceBotsResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceRetentionSettingsTypeDef = TypedDict(
     "AppInstanceRetentionSettingsTypeDef",
     {
         "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
     total=False,
 )
 
-ListAppInstancesResponseTypeDef = TypedDict(
-    "ListAppInstancesResponseTypeDef",
-    {
-        "AppInstances": List[AppInstanceSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
-    {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceUserEndpointSummaryTypeDef = TypedDict(
     "AppInstanceUserEndpointSummaryTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
         "Name": str,
         "Type": AppInstanceUserEndpointTypeType,
@@ -681,24 +572,14 @@
 class RegisterAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredRegisterAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalRegisterAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
 
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceUserTypeDef = TypedDict(
     "AppInstanceUserTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
         "CreatedTimestamp": datetime,
@@ -726,20 +607,139 @@
 class PutAppInstanceUserExpirationSettingsRequestRequestTypeDef(
     _RequiredPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
     _OptionalPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
 ):
     pass
 
 
+CreateAppInstanceAdminResponseTypeDef = TypedDict(
+    "CreateAppInstanceAdminResponseTypeDef",
+    {
+        "AppInstanceAdmin": IdentityTypeDef,
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceBotResponseTypeDef = TypedDict(
+    "CreateAppInstanceBotResponseTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
+    {
+        "AppInstance": AppInstanceTypeDef,
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
+ListAppInstanceBotsResponseTypeDef = TypedDict(
+    "ListAppInstanceBotsResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppInstancesResponseTypeDef = TypedDict(
+    "ListAppInstancesResponseTypeDef",
+    {
+        "AppInstances": List[AppInstanceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppInstanceUserExpirationSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
     {
         "AppInstanceUserArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceBotResponseTypeDef = TypedDict(
+    "UpdateAppInstanceBotResponseTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -789,15 +789,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -829,32 +829,32 @@
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -863,40 +863,40 @@
 )
 
 PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstanceUserEndpointsResponseTypeDef = TypedDict(
     "ListAppInstanceUserEndpointsResponseTypeDef",
     {
         "AppInstanceUserEndpoints": List[AppInstanceUserEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceUserEndpointResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     {
         "AppInstanceUserEndpoint": AppInstanceUserEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Lex": LexConfigurationTypeDef,
@@ -966,10 +966,10 @@
     pass
 
 
 DescribeAppInstanceBotResponseTypeDef = TypedDict(
     "DescribeAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBot": AppInstanceBotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity/type_defs.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_identity.type_defs import IdentityTypeDef
 
-    data: IdentityTypeDef = {...}
+    data: IdentityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -40,61 +40,61 @@
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
     "EndpointAttributesTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateAppInstanceBotResponseTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceBotRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeregisterAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceAdminRequestRequestTypeDef",
     "DescribeAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceRequestRequestTypeDef",
     "DescribeAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceUserRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "InvokedByTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceBotsRequestRequestTypeDef",
     "ListAppInstanceUserEndpointsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppInstanceBotResponseTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserEndpointRequestRequestTypeDef",
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "ListAppInstanceBotsResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
     "AppInstanceUserEndpointSummaryTypeDef",
     "AppInstanceUserEndpointTypeDef",
     "RegisterAppInstanceUserEndpointRequestRequestTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
     "AppInstanceUserTypeDef",
     "PutAppInstanceUserExpirationSettingsRequestRequestTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateAppInstanceBotResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAppInstanceBotsResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    "UpdateAppInstanceBotResponseTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "LexConfigurationTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
@@ -218,43 +218,30 @@
     "CreateAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
         "AppInstanceArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-CreateAppInstanceBotResponseTypeDef = TypedDict(
-    "CreateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
 DeleteAppInstanceAdminRequestRequestTypeDef = TypedDict(
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
@@ -324,21 +311,14 @@
 DescribeAppInstanceUserRequestRequestTypeDef = TypedDict(
     "DescribeAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
@@ -446,67 +426,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAppInstanceBotResponseTypeDef = TypedDict(
-    "UpdateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAppInstanceRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
     },
 )
@@ -521,40 +465,23 @@
 
 class UpdateAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
-UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -565,58 +492,22 @@
         "Admin": IdentityTypeDef,
         "AppInstanceArn": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-CreateAppInstanceAdminResponseTypeDef = TypedDict(
-    "CreateAppInstanceAdminResponseTypeDef",
-    {
-        "AppInstanceAdmin": IdentityTypeDef,
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAppInstanceBotsResponseTypeDef = TypedDict(
-    "ListAppInstanceBotsResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceRetentionSettingsTypeDef = TypedDict(
     "AppInstanceRetentionSettingsTypeDef",
     {
         "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
     total=False,
 )
 
-ListAppInstancesResponseTypeDef = TypedDict(
-    "ListAppInstancesResponseTypeDef",
-    {
-        "AppInstances": List[AppInstanceSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
-    {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceUserEndpointSummaryTypeDef = TypedDict(
     "AppInstanceUserEndpointSummaryTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
         "Name": str,
         "Type": AppInstanceUserEndpointTypeType,
@@ -664,24 +555,14 @@
 
 class RegisterAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredRegisterAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalRegisterAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AppInstanceUserTypeDef = TypedDict(
     "AppInstanceUserTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
         "CreatedTimestamp": datetime,
@@ -707,20 +588,139 @@
 
 class PutAppInstanceUserExpirationSettingsRequestRequestTypeDef(
     _RequiredPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
     _OptionalPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
 ):
     pass
 
+CreateAppInstanceAdminResponseTypeDef = TypedDict(
+    "CreateAppInstanceAdminResponseTypeDef",
+    {
+        "AppInstanceAdmin": IdentityTypeDef,
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceBotResponseTypeDef = TypedDict(
+    "CreateAppInstanceBotResponseTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
+    {
+        "AppInstance": AppInstanceTypeDef,
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
+ListAppInstanceBotsResponseTypeDef = TypedDict(
+    "ListAppInstanceBotsResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppInstancesResponseTypeDef = TypedDict(
+    "ListAppInstancesResponseTypeDef",
+    {
+        "AppInstances": List[AppInstanceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppInstanceUserExpirationSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
     {
         "AppInstanceUserArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceBotResponseTypeDef = TypedDict(
+    "UpdateAppInstanceBotResponseTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -766,15 +766,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -804,32 +804,32 @@
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -838,40 +838,40 @@
 )
 
 PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstanceUserEndpointsResponseTypeDef = TypedDict(
     "ListAppInstanceUserEndpointsResponseTypeDef",
     {
         "AppInstanceUserEndpoints": List[AppInstanceUserEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceUserEndpointResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     {
         "AppInstanceUserEndpoint": AppInstanceUserEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Lex": LexConfigurationTypeDef,
@@ -937,10 +937,10 @@
 ):
     pass
 
 DescribeAppInstanceBotResponseTypeDef = TypedDict(
     "DescribeAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBot": AppInstanceBotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-identity
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-identity type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-identity type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-identity"></a>
 
 # types-aiobotocore-chime-sdk-identity
 
 [![PyPI - types-aiobotocore-chime-sdk-identity](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-identity?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-identity)](https://pepy.tech/project/types-aiobotocore-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
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
@@ -288,80 +287,80 @@
 )
 
 
 def check_value(value: AllowMessagesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_identity.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_identity.type_defs import (
     IdentityTypeDef,
     AppInstanceBotSummaryTypeDef,
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceBotResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAppInstanceBotsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
     PutAppInstanceUserExpirationSettingsResponseTypeDef,
+    RegisterAppInstanceUserEndpointResponseTypeDef,
+    UpdateAppInstanceBotResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserEndpointResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
@@ -375,15 +374,15 @@
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
     UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityTypeDef:
+def get_value() -> IdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-amplifybackend-2.5.2.tar.gz` & `tmp/types-aiobotocore-amplifybackend-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplifybackend-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplifybackend-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
```

## Comparing `types-aiobotocore-amplifybackend-2.5.2.tar` & `types-aiobotocore-amplifybackend-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.837605 types-aiobotocore-amplifybackend-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-07-08 01:43:09.837605 types-aiobotocore-amplifybackend-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.837605 types-aiobotocore-amplifybackend-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24798 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24757 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38958 2023-07-08 01:25:27.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-07-08 01:25:26.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:25.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.837605 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-07-08 01:43:09.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:09.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:09.000000 types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.837667 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44462 2023-08-02 14:32:53.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44397 2023-08-02 14:32:52.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/LICENSE` & `types-aiobotocore-amplifybackend-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/PKG-INFO` & `types-aiobotocore-amplifybackend-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifybackend
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AmplifyBackend 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AmplifyBackend 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore amplifybackend type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amplifybackend"></a>
 
 # types-aiobotocore-amplifybackend
 
 [![PyPI - types-aiobotocore-amplifybackend](https://img.shields.io/pypi/v/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplifybackend?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplifybackend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifybackend)](https://pepy.tech/project/types-aiobotocore-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AmplifyBackend 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [types-aiobotocore-amplifybackend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/).
 
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
@@ -323,35 +322,38 @@
 )
 
 
 def check_value(value: AdditionalConstraintsElementType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplifybackend.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplifybackend.type_defs import (
     BackendAPIAppSyncAuthSettingsTypeDef,
     BackendAPIConflictResolutionTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
+    BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
+    CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
     CreateTokenRequestRequestTypeDef,
     DeleteBackendAuthRequestRequestTypeDef,
     DeleteBackendRequestRequestTypeDef,
     DeleteBackendStorageRequestRequestTypeDef,
@@ -373,16 +375,16 @@
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
     BackendAPIAuthTypeTypeDef,
     SocialProviderSettingsTypeDef,
-    CreateBackendStorageResourceConfigTypeDef,
     GetBackendStorageResourceConfigTypeDef,
+    CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResponseTypeDef,
@@ -406,42 +408,49 @@
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
+    CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
     UpdateBackendConfigRequestRequestTypeDef,
     UpdateBackendConfigResponseTypeDef,
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
+    CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
-    CreateBackendStorageRequestRequestTypeDef,
     GetBackendStorageResponseTypeDef,
+    CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
+    GetBackendAPIResponseTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
-    GetBackendAPIResponseTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
+    CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
-    CreateBackendAuthRequestRequestTypeDef,
     GetBackendAuthResponseTypeDef,
+    CreateBackendAuthRequestRequestTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_value() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/README.md` & `types-aiobotocore-amplifybackend-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-amplifybackend"></a>
 
 # types-aiobotocore-amplifybackend
 
 [![PyPI - types-aiobotocore-amplifybackend](https://img.shields.io/pypi/v/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplifybackend?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplifybackend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifybackend)](https://pepy.tech/project/types-aiobotocore-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AmplifyBackend 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [types-aiobotocore-amplifybackend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/).
 
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
@@ -290,35 +290,38 @@
 )
 
 
 def check_value(value: AdditionalConstraintsElementType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplifybackend.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplifybackend.type_defs import (
     BackendAPIAppSyncAuthSettingsTypeDef,
     BackendAPIConflictResolutionTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
+    BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
+    CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
     CreateTokenRequestRequestTypeDef,
     DeleteBackendAuthRequestRequestTypeDef,
     DeleteBackendRequestRequestTypeDef,
     DeleteBackendStorageRequestRequestTypeDef,
@@ -340,16 +343,16 @@
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
     BackendAPIAuthTypeTypeDef,
     SocialProviderSettingsTypeDef,
-    CreateBackendStorageResourceConfigTypeDef,
     GetBackendStorageResourceConfigTypeDef,
+    CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResponseTypeDef,
@@ -373,42 +376,49 @@
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
+    CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
     UpdateBackendConfigRequestRequestTypeDef,
     UpdateBackendConfigResponseTypeDef,
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
+    CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
-    CreateBackendStorageRequestRequestTypeDef,
     GetBackendStorageResponseTypeDef,
+    CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
+    GetBackendAPIResponseTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
-    GetBackendAPIResponseTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
+    CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
-    CreateBackendAuthRequestRequestTypeDef,
     GetBackendAuthResponseTypeDef,
+    CreateBackendAuthRequestRequestTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_value() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/setup.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplifybackend",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AmplifyBackend 2.5.2 service generated with"
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
-    keywords="aiobotocore amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore amplifybackend type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_amplifybackend": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/"
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/__init__.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/__init__.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/__main__.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AmplifyBackend 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AmplifyBackend 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
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

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/client.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
-    BackendAPIResourceConfigTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
-    CreateBackendAuthResourceConfigTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
     DeleteBackendAPIResponseTypeDef,
@@ -146,30 +146,30 @@
         """
 
     async def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef,
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_api)
         """
 
     async def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
+        ResourceConfig: CreateBackendAuthResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_auth)
@@ -221,15 +221,15 @@
 
     async def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_api)
         """
@@ -303,15 +303,15 @@
 
     async def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#get_backend_api)
         """
@@ -442,15 +442,15 @@
 
     async def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/client.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
-    BackendAPIResourceConfigTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
-    CreateBackendAuthResourceConfigTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
     DeleteBackendAPIResponseTypeDef,
@@ -137,29 +137,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend)
         """
     async def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef,
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_api)
         """
     async def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
+        ResourceConfig: CreateBackendAuthResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_auth)
@@ -206,15 +206,15 @@
         """
     async def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_api)
         """
@@ -281,15 +281,15 @@
         """
     async def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#get_backend_api)
         """
@@ -408,15 +408,15 @@
         """
     async def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/literals.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/literals.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/paginator.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/paginator.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/type_defs.py` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalConstraintsElementType,
     AuthenticatedElementType,
     AuthResourcesType,
     DeliveryMethodType,
     MFAModeType,
@@ -36,28 +36,30 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BackendAPIAppSyncAuthSettingsTypeDef",
     "BackendAPIConflictResolutionTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
+    "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
+    "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "DeleteBackendAuthRequestRequestTypeDef",
     "DeleteBackendRequestRequestTypeDef",
     "DeleteBackendStorageRequestRequestTypeDef",
@@ -79,16 +81,16 @@
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
     "BackendAPIAuthTypeTypeDef",
     "SocialProviderSettingsTypeDef",
-    "CreateBackendStorageResourceConfigTypeDef",
     "GetBackendStorageResourceConfigTypeDef",
+    "CreateBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
     "CreateBackendConfigResponseTypeDef",
     "CreateBackendResponseTypeDef",
     "CreateBackendStorageResponseTypeDef",
@@ -112,37 +114,44 @@
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
+    "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
     "UpdateBackendConfigRequestRequestTypeDef",
     "UpdateBackendConfigResponseTypeDef",
+    "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
+    "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
-    "CreateBackendStorageRequestRequestTypeDef",
     "GetBackendStorageResponseTypeDef",
+    "CreateBackendStorageRequestRequestTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
+    "GetBackendAPIResponseTypeDef",
+    "BackendAPIResourceConfigUnionTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
-    "GetBackendAPIResponseTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
+    "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
+    "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
-    "CreateBackendAuthRequestRequestTypeDef",
     "GetBackendAuthResponseTypeDef",
+    "CreateBackendAuthRequestRequestTypeDef",
+    "CreateBackendAuthResourceConfigUnionTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
@@ -201,20 +210,37 @@
         "Operation": str,
         "Status": str,
         "UpdateTime": str,
     },
     total=False,
 )
 
-
 class BackendJobRespObjTypeDef(
     _RequiredBackendJobRespObjTypeDef, _OptionalBackendJobRespObjTypeDef
 ):
     pass
 
+_RequiredBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_RequiredBackendStoragePermissionsOutputTypeDef",
+    {
+        "Authenticated": List[AuthenticatedElementType],
+    },
+)
+_OptionalBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_OptionalBackendStoragePermissionsOutputTypeDef",
+    {
+        "UnAuthenticated": List[UnAuthenticatedElementType],
+    },
+    total=False,
+)
+
+class BackendStoragePermissionsOutputTypeDef(
+    _RequiredBackendStoragePermissionsOutputTypeDef, _OptionalBackendStoragePermissionsOutputTypeDef
+):
+    pass
 
 _RequiredBackendStoragePermissionsTypeDef = TypedDict(
     "_RequiredBackendStoragePermissionsTypeDef",
     {
         "Authenticated": Sequence[AuthenticatedElementType],
     },
 )
@@ -222,21 +248,19 @@
     "_OptionalBackendStoragePermissionsTypeDef",
     {
         "UnAuthenticated": Sequence[UnAuthenticatedElementType],
     },
     total=False,
 )
 
-
 class BackendStoragePermissionsTypeDef(
     _RequiredBackendStoragePermissionsTypeDef, _OptionalBackendStoragePermissionsTypeDef
 ):
     pass
 
-
 CloneBackendRequestRequestTypeDef = TypedDict(
     "CloneBackendRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "TargetEnvironmentName": str,
     },
@@ -274,67 +298,92 @@
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "MfaTypes": List[MfaTypesElementType],
+        "SmsMessage": str,
+    },
+    total=False,
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "MfaTypes": Sequence[MfaTypesElementType],
         "SmsMessage": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "MinimumLength": float,
+    },
+)
+_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "AdditionalConstraints": List[AdditionalConstraintsElementType],
+    },
+    total=False,
+)
+
+class CreateBackendAuthPasswordPolicyConfigOutputTypeDef(
+    _RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+    _OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "MinimumLength": float,
     },
 )
 _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_OptionalCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "AdditionalConstraints": Sequence[AdditionalConstraintsElementType],
     },
     total=False,
 )
 
-
 class CreateBackendAuthPasswordPolicyConfigTypeDef(
     _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef,
     _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef,
 ):
     pass
 
-
 _RequiredCreateBackendConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalCreateBackendConfigRequestRequestTypeDef = TypedDict(
     "_OptionalCreateBackendConfigRequestRequestTypeDef",
     {
         "BackendManagerAppId": str,
     },
     total=False,
 )
 
-
 class CreateBackendConfigRequestRequestTypeDef(
     _RequiredCreateBackendConfigRequestRequestTypeDef,
     _OptionalCreateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateBackendRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackendRequestRequestTypeDef",
     {
         "AppId": str,
         "AppName": str,
         "BackendEnvironmentName": str,
     },
@@ -344,21 +393,19 @@
     {
         "ResourceConfig": Mapping[str, Any],
         "ResourceName": str,
     },
     total=False,
 )
 
-
 class CreateBackendRequestRequestTypeDef(
     _RequiredCreateBackendRequestRequestTypeDef, _OptionalCreateBackendRequestRequestTypeDef
 ):
     pass
 
-
 CreateTokenRequestRequestTypeDef = TypedDict(
     "CreateTokenRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -443,21 +490,19 @@
     "_OptionalGetBackendRequestRequestTypeDef",
     {
         "BackendEnvironmentName": str,
     },
     total=False,
 )
 
-
 class GetBackendRequestRequestTypeDef(
     _RequiredGetBackendRequestRequestTypeDef, _OptionalGetBackendRequestRequestTypeDef
 ):
     pass
 
-
 GetBackendStorageRequestRequestTypeDef = TypedDict(
     "GetBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -485,21 +530,19 @@
     "_OptionalImportBackendAuthRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
     total=False,
 )
 
-
 class ImportBackendAuthRequestRequestTypeDef(
     _RequiredImportBackendAuthRequestRequestTypeDef, _OptionalImportBackendAuthRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredImportBackendStorageRequestRequestTypeDef = TypedDict(
     "_RequiredImportBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ServiceName": Literal["S3"],
     },
@@ -508,22 +551,20 @@
     "_OptionalImportBackendStorageRequestRequestTypeDef",
     {
         "BucketName": str,
     },
     total=False,
 )
 
-
 class ImportBackendStorageRequestRequestTypeDef(
     _RequiredImportBackendStorageRequestRequestTypeDef,
     _OptionalImportBackendStorageRequestRequestTypeDef,
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -545,21 +586,19 @@
         "NextToken": str,
         "Operation": str,
         "Status": str,
     },
     total=False,
 )
 
-
 class ListBackendJobsRequestRequestTypeDef(
     _RequiredListBackendJobsRequestRequestTypeDef, _OptionalListBackendJobsRequestRequestTypeDef
 ):
     pass
 
-
 ListS3BucketsRequestRequestTypeDef = TypedDict(
     "ListS3BucketsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -594,21 +633,19 @@
     "_OptionalRemoveAllBackendsRequestRequestTypeDef",
     {
         "CleanAmplifyApp": bool,
     },
     total=False,
 )
 
-
 class RemoveAllBackendsRequestRequestTypeDef(
     _RequiredRemoveAllBackendsRequestRequestTypeDef, _OptionalRemoveAllBackendsRequestRequestTypeDef
 ):
     pass
 
-
 RemoveBackendConfigRequestRequestTypeDef = TypedDict(
     "RemoveBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -642,21 +679,19 @@
     {
         "Operation": str,
         "Status": str,
     },
     total=False,
 )
 
-
 class UpdateBackendJobRequestRequestTypeDef(
     _RequiredUpdateBackendJobRequestRequestTypeDef, _OptionalUpdateBackendJobRequestRequestTypeDef
 ):
     pass
 
-
 BackendAPIAuthTypeTypeDef = TypedDict(
     "BackendAPIAuthTypeTypeDef",
     {
         "Mode": ModeType,
         "Settings": BackendAPIAppSyncAuthSettingsTypeDef,
     },
     total=False,
@@ -669,60 +704,56 @@
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredCreateBackendStorageResourceConfigTypeDef",
+_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredGetBackendStorageResourceConfigTypeDef",
     {
-        "Permissions": BackendStoragePermissionsTypeDef,
+        "Imported": bool,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalCreateBackendStorageResourceConfigTypeDef",
+_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalGetBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
+        "Permissions": BackendStoragePermissionsOutputTypeDef,
     },
     total=False,
 )
 
-
-class CreateBackendStorageResourceConfigTypeDef(
-    _RequiredCreateBackendStorageResourceConfigTypeDef,
-    _OptionalCreateBackendStorageResourceConfigTypeDef,
+class GetBackendStorageResourceConfigTypeDef(
+    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
 ):
     pass
 
-
-_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredGetBackendStorageResourceConfigTypeDef",
+_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredCreateBackendStorageResourceConfigTypeDef",
     {
-        "Imported": bool,
+        "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalGetBackendStorageResourceConfigTypeDef",
+_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalCreateBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
-        "Permissions": BackendStoragePermissionsTypeDef,
     },
     total=False,
 )
 
-
-class GetBackendStorageResourceConfigTypeDef(
-    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
+class CreateBackendStorageResourceConfigTypeDef(
+    _RequiredCreateBackendStorageResourceConfigTypeDef,
+    _OptionalCreateBackendStorageResourceConfigTypeDef,
 ):
     pass
 
-
 UpdateBackendStorageResourceConfigTypeDef = TypedDict(
     "UpdateBackendStorageResourceConfigTypeDef",
     {
         "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
@@ -1049,22 +1080,20 @@
     {
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateBackendAuthForgotPasswordConfigTypeDef(
     _RequiredCreateBackendAuthForgotPasswordConfigTypeDef,
     _OptionalCreateBackendAuthForgotPasswordConfigTypeDef,
 ):
     pass
 
-
 _RequiredCreateBackendAuthVerificationMessageConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthVerificationMessageConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
     },
 )
 _OptionalCreateBackendAuthVerificationMessageConfigTypeDef = TypedDict(
@@ -1072,22 +1101,20 @@
     {
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredCreateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalCreateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
-
 UpdateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
@@ -1105,21 +1132,39 @@
     {
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredUpdateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalUpdateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
+_RequiredCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "MFAMode": MFAModeType,
+    },
+)
+_OptionalCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "Settings": SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthMFAConfigOutputTypeDef(
+    _RequiredCreateBackendAuthMFAConfigOutputTypeDef,
+    _OptionalCreateBackendAuthMFAConfigOutputTypeDef,
+):
+    pass
 
 _RequiredCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
     },
 )
@@ -1127,21 +1172,19 @@
     "_OptionalCreateBackendAuthMFAConfigTypeDef",
     {
         "Settings": SettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateBackendAuthMFAConfigTypeDef(
     _RequiredCreateBackendAuthMFAConfigTypeDef, _OptionalCreateBackendAuthMFAConfigTypeDef
 ):
     pass
 
-
 UpdateBackendAuthMFAConfigTypeDef = TypedDict(
     "UpdateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
         "Settings": SettingsTypeDef,
     },
     total=False,
@@ -1161,22 +1204,20 @@
         "Operation": str,
         "Status": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListBackendJobsRequestListBackendJobsPaginateTypeDef(
     _RequiredListBackendJobsRequestListBackendJobsPaginateTypeDef,
     _OptionalListBackendJobsRequestListBackendJobsPaginateTypeDef,
 ):
     pass
 
-
 ListS3BucketsResponseTypeDef = TypedDict(
     "ListS3BucketsResponseTypeDef",
     {
         "Buckets": List[S3BucketInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1192,46 +1233,81 @@
     "_OptionalUpdateBackendConfigRequestRequestTypeDef",
     {
         "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBackendConfigRequestRequestTypeDef(
     _RequiredUpdateBackendConfigRequestRequestTypeDef,
     _OptionalUpdateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateBackendConfigResponseTypeDef = TypedDict(
     "UpdateBackendConfigResponseTypeDef",
     {
         "AppId": str,
         "BackendManagerAppId": str,
         "Error": str,
         "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BackendAPIResourceConfigOutputTypeDef = TypedDict(
+    "BackendAPIResourceConfigOutputTypeDef",
+    {
+        "AdditionalAuthTypes": List[BackendAPIAuthTypeTypeDef],
+        "ApiName": str,
+        "ConflictResolution": BackendAPIConflictResolutionTypeDef,
+        "DefaultAuthType": BackendAPIAuthTypeTypeDef,
+        "Service": str,
+        "TransformSchema": str,
+    },
+    total=False,
+)
+
 BackendAPIResourceConfigTypeDef = TypedDict(
     "BackendAPIResourceConfigTypeDef",
     {
         "AdditionalAuthTypes": Sequence[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
         "ConflictResolution": BackendAPIConflictResolutionTypeDef,
         "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "OAuthGrantType": OAuthGrantTypeType,
+        "OAuthScopes": List[OAuthScopesElementType],
+        "RedirectSignInURIs": List[str],
+        "RedirectSignOutURIs": List[str],
+    },
+)
+_OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "DomainPrefix": str,
+        "SocialProviderSettings": SocialProviderSettingsTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthOAuthConfigOutputTypeDef(
+    _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
+    _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthOAuthConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthOAuthConfigTypeDef",
     {
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
@@ -1242,65 +1318,78 @@
     {
         "DomainPrefix": str,
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateBackendAuthOAuthConfigTypeDef(
     _RequiredCreateBackendAuthOAuthConfigTypeDef, _OptionalCreateBackendAuthOAuthConfigTypeDef
 ):
     pass
 
-
 UpdateBackendAuthOAuthConfigTypeDef = TypedDict(
     "UpdateBackendAuthOAuthConfigTypeDef",
     {
         "DomainPrefix": str,
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-CreateBackendStorageRequestRequestTypeDef = TypedDict(
-    "CreateBackendStorageRequestRequestTypeDef",
+GetBackendStorageResponseTypeDef = TypedDict(
+    "GetBackendStorageResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendStorageResponseTypeDef = TypedDict(
-    "GetBackendStorageResponseTypeDef",
+CreateBackendStorageRequestRequestTypeDef = TypedDict(
+    "CreateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBackendStorageRequestRequestTypeDef = TypedDict(
     "UpdateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
+GetBackendAPIResponseTypeDef = TypedDict(
+    "GetBackendAPIResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendEnvironmentName": str,
+        "Error": str,
+        "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BackendAPIResourceConfigUnionTypeDef = Union[
+    BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+]
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1319,21 +1408,19 @@
     "_OptionalDeleteBackendAPIRequestRequestTypeDef",
     {
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
     },
     total=False,
 )
 
-
 class DeleteBackendAPIRequestRequestTypeDef(
     _RequiredDeleteBackendAPIRequestRequestTypeDef, _OptionalDeleteBackendAPIRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredGetBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1342,33 +1429,19 @@
     "_OptionalGetBackendAPIRequestRequestTypeDef",
     {
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetBackendAPIRequestRequestTypeDef(
     _RequiredGetBackendAPIRequestRequestTypeDef, _OptionalGetBackendAPIRequestRequestTypeDef
 ):
     pass
 
-
-GetBackendAPIResponseTypeDef = TypedDict(
-    "GetBackendAPIResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": BackendAPIResourceConfigTypeDef,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1377,20 +1450,44 @@
     "_OptionalUpdateBackendAPIRequestRequestTypeDef",
     {
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBackendAPIRequestRequestTypeDef(
     _RequiredUpdateBackendAPIRequestRequestTypeDef, _OptionalUpdateBackendAPIRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "RequiredSignUpAttributes": List[RequiredSignUpAttributesElementType],
+        "SignInMethod": SignInMethodType,
+        "UserPoolName": str,
+    },
+)
+_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "ForgotPassword": CreateBackendAuthForgotPasswordConfigTypeDef,
+        "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
+        "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
+        "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+        "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthUserPoolConfigOutputTypeDef(
+    _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
+    _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
+):
+    pass
 
 _RequiredCreateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthUserPoolConfigTypeDef",
     {
         "RequiredSignUpAttributes": Sequence[RequiredSignUpAttributesElementType],
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
@@ -1404,33 +1501,53 @@
         "OAuth": CreateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
-
 class CreateBackendAuthUserPoolConfigTypeDef(
     _RequiredCreateBackendAuthUserPoolConfigTypeDef, _OptionalCreateBackendAuthUserPoolConfigTypeDef
 ):
     pass
 
-
 UpdateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "UpdateBackendAuthUserPoolConfigTypeDef",
     {
         "ForgotPassword": UpdateBackendAuthForgotPasswordConfigTypeDef,
         "Mfa": UpdateBackendAuthMFAConfigTypeDef,
         "OAuth": UpdateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": UpdateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": UpdateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "AuthResources": AuthResourcesType,
+        "Service": Literal["COGNITO"],
+        "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
+    },
+)
+_OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthResourceConfigOutputTypeDef(
+    _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
+    _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1439,21 +1556,19 @@
     "_OptionalCreateBackendAuthResourceConfigTypeDef",
     {
         "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
     },
     total=False,
 )
 
-
 class CreateBackendAuthResourceConfigTypeDef(
     _RequiredCreateBackendAuthResourceConfigTypeDef, _OptionalCreateBackendAuthResourceConfigTypeDef
 ):
     pass
 
-
 _RequiredUpdateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredUpdateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": UpdateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1462,43 +1577,44 @@
     "_OptionalUpdateBackendAuthResourceConfigTypeDef",
     {
         "IdentityPoolConfigs": UpdateBackendAuthIdentityPoolConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBackendAuthResourceConfigTypeDef(
     _RequiredUpdateBackendAuthResourceConfigTypeDef, _OptionalUpdateBackendAuthResourceConfigTypeDef
 ):
     pass
 
-
-CreateBackendAuthRequestRequestTypeDef = TypedDict(
-    "CreateBackendAuthRequestRequestTypeDef",
+GetBackendAuthResponseTypeDef = TypedDict(
+    "GetBackendAuthResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
+        "Error": str,
+        "ResourceConfig": CreateBackendAuthResourceConfigOutputTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendAuthResponseTypeDef = TypedDict(
-    "GetBackendAuthResponseTypeDef",
+CreateBackendAuthRequestRequestTypeDef = TypedDict(
+    "CreateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateBackendAuthResourceConfigUnionTypeDef = Union[
+    CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
+]
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend/type_defs.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalConstraintsElementType,
     AuthenticatedElementType,
     AuthResourcesType,
     DeliveryMethodType,
     MFAModeType,
@@ -36,27 +36,31 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BackendAPIAppSyncAuthSettingsTypeDef",
     "BackendAPIConflictResolutionTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
+    "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
+    "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "DeleteBackendAuthRequestRequestTypeDef",
     "DeleteBackendRequestRequestTypeDef",
     "DeleteBackendStorageRequestRequestTypeDef",
@@ -78,16 +82,16 @@
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
     "BackendAPIAuthTypeTypeDef",
     "SocialProviderSettingsTypeDef",
-    "CreateBackendStorageResourceConfigTypeDef",
     "GetBackendStorageResourceConfigTypeDef",
+    "CreateBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
     "CreateBackendConfigResponseTypeDef",
     "CreateBackendResponseTypeDef",
     "CreateBackendStorageResponseTypeDef",
@@ -111,37 +115,44 @@
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
+    "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
     "UpdateBackendConfigRequestRequestTypeDef",
     "UpdateBackendConfigResponseTypeDef",
+    "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
+    "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
-    "CreateBackendStorageRequestRequestTypeDef",
     "GetBackendStorageResponseTypeDef",
+    "CreateBackendStorageRequestRequestTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
+    "GetBackendAPIResponseTypeDef",
+    "BackendAPIResourceConfigUnionTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
-    "GetBackendAPIResponseTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
+    "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
+    "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
-    "CreateBackendAuthRequestRequestTypeDef",
     "GetBackendAuthResponseTypeDef",
+    "CreateBackendAuthRequestRequestTypeDef",
+    "CreateBackendAuthResourceConfigUnionTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
@@ -200,38 +211,63 @@
         "Operation": str,
         "Status": str,
         "UpdateTime": str,
     },
     total=False,
 )
 
+
 class BackendJobRespObjTypeDef(
     _RequiredBackendJobRespObjTypeDef, _OptionalBackendJobRespObjTypeDef
 ):
     pass
 
+
+_RequiredBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_RequiredBackendStoragePermissionsOutputTypeDef",
+    {
+        "Authenticated": List[AuthenticatedElementType],
+    },
+)
+_OptionalBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_OptionalBackendStoragePermissionsOutputTypeDef",
+    {
+        "UnAuthenticated": List[UnAuthenticatedElementType],
+    },
+    total=False,
+)
+
+
+class BackendStoragePermissionsOutputTypeDef(
+    _RequiredBackendStoragePermissionsOutputTypeDef, _OptionalBackendStoragePermissionsOutputTypeDef
+):
+    pass
+
+
 _RequiredBackendStoragePermissionsTypeDef = TypedDict(
     "_RequiredBackendStoragePermissionsTypeDef",
     {
         "Authenticated": Sequence[AuthenticatedElementType],
     },
 )
 _OptionalBackendStoragePermissionsTypeDef = TypedDict(
     "_OptionalBackendStoragePermissionsTypeDef",
     {
         "UnAuthenticated": Sequence[UnAuthenticatedElementType],
     },
     total=False,
 )
 
+
 class BackendStoragePermissionsTypeDef(
     _RequiredBackendStoragePermissionsTypeDef, _OptionalBackendStoragePermissionsTypeDef
 ):
     pass
 
+
 CloneBackendRequestRequestTypeDef = TypedDict(
     "CloneBackendRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "TargetEnvironmentName": str,
     },
@@ -269,63 +305,98 @@
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "MfaTypes": List[MfaTypesElementType],
+        "SmsMessage": str,
+    },
+    total=False,
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "MfaTypes": Sequence[MfaTypesElementType],
         "SmsMessage": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "MinimumLength": float,
+    },
+)
+_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "AdditionalConstraints": List[AdditionalConstraintsElementType],
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthPasswordPolicyConfigOutputTypeDef(
+    _RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+    _OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "MinimumLength": float,
     },
 )
 _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_OptionalCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "AdditionalConstraints": Sequence[AdditionalConstraintsElementType],
     },
     total=False,
 )
 
+
 class CreateBackendAuthPasswordPolicyConfigTypeDef(
     _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef,
     _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef,
 ):
     pass
 
+
 _RequiredCreateBackendConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalCreateBackendConfigRequestRequestTypeDef = TypedDict(
     "_OptionalCreateBackendConfigRequestRequestTypeDef",
     {
         "BackendManagerAppId": str,
     },
     total=False,
 )
 
+
 class CreateBackendConfigRequestRequestTypeDef(
     _RequiredCreateBackendConfigRequestRequestTypeDef,
     _OptionalCreateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateBackendRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackendRequestRequestTypeDef",
     {
         "AppId": str,
         "AppName": str,
         "BackendEnvironmentName": str,
     },
@@ -335,19 +406,21 @@
     {
         "ResourceConfig": Mapping[str, Any],
         "ResourceName": str,
     },
     total=False,
 )
 
+
 class CreateBackendRequestRequestTypeDef(
     _RequiredCreateBackendRequestRequestTypeDef, _OptionalCreateBackendRequestRequestTypeDef
 ):
     pass
 
+
 CreateTokenRequestRequestTypeDef = TypedDict(
     "CreateTokenRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -432,19 +505,21 @@
     "_OptionalGetBackendRequestRequestTypeDef",
     {
         "BackendEnvironmentName": str,
     },
     total=False,
 )
 
+
 class GetBackendRequestRequestTypeDef(
     _RequiredGetBackendRequestRequestTypeDef, _OptionalGetBackendRequestRequestTypeDef
 ):
     pass
 
+
 GetBackendStorageRequestRequestTypeDef = TypedDict(
     "GetBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -472,19 +547,21 @@
     "_OptionalImportBackendAuthRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
     total=False,
 )
 
+
 class ImportBackendAuthRequestRequestTypeDef(
     _RequiredImportBackendAuthRequestRequestTypeDef, _OptionalImportBackendAuthRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredImportBackendStorageRequestRequestTypeDef = TypedDict(
     "_RequiredImportBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ServiceName": Literal["S3"],
     },
@@ -493,20 +570,22 @@
     "_OptionalImportBackendStorageRequestRequestTypeDef",
     {
         "BucketName": str,
     },
     total=False,
 )
 
+
 class ImportBackendStorageRequestRequestTypeDef(
     _RequiredImportBackendStorageRequestRequestTypeDef,
     _OptionalImportBackendStorageRequestRequestTypeDef,
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -528,19 +607,21 @@
         "NextToken": str,
         "Operation": str,
         "Status": str,
     },
     total=False,
 )
 
+
 class ListBackendJobsRequestRequestTypeDef(
     _RequiredListBackendJobsRequestRequestTypeDef, _OptionalListBackendJobsRequestRequestTypeDef
 ):
     pass
 
+
 ListS3BucketsRequestRequestTypeDef = TypedDict(
     "ListS3BucketsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -575,19 +656,21 @@
     "_OptionalRemoveAllBackendsRequestRequestTypeDef",
     {
         "CleanAmplifyApp": bool,
     },
     total=False,
 )
 
+
 class RemoveAllBackendsRequestRequestTypeDef(
     _RequiredRemoveAllBackendsRequestRequestTypeDef, _OptionalRemoveAllBackendsRequestRequestTypeDef
 ):
     pass
 
+
 RemoveBackendConfigRequestRequestTypeDef = TypedDict(
     "RemoveBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -621,19 +704,21 @@
     {
         "Operation": str,
         "Status": str,
     },
     total=False,
 )
 
+
 class UpdateBackendJobRequestRequestTypeDef(
     _RequiredUpdateBackendJobRequestRequestTypeDef, _OptionalUpdateBackendJobRequestRequestTypeDef
 ):
     pass
 
+
 BackendAPIAuthTypeTypeDef = TypedDict(
     "BackendAPIAuthTypeTypeDef",
     {
         "Mode": ModeType,
         "Settings": BackendAPIAppSyncAuthSettingsTypeDef,
     },
     total=False,
@@ -646,56 +731,60 @@
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredCreateBackendStorageResourceConfigTypeDef",
+_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredGetBackendStorageResourceConfigTypeDef",
     {
-        "Permissions": BackendStoragePermissionsTypeDef,
+        "Imported": bool,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalCreateBackendStorageResourceConfigTypeDef",
+_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalGetBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
+        "Permissions": BackendStoragePermissionsOutputTypeDef,
     },
     total=False,
 )
 
-class CreateBackendStorageResourceConfigTypeDef(
-    _RequiredCreateBackendStorageResourceConfigTypeDef,
-    _OptionalCreateBackendStorageResourceConfigTypeDef,
+
+class GetBackendStorageResourceConfigTypeDef(
+    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
 ):
     pass
 
-_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredGetBackendStorageResourceConfigTypeDef",
+
+_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredCreateBackendStorageResourceConfigTypeDef",
     {
-        "Imported": bool,
+        "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalGetBackendStorageResourceConfigTypeDef",
+_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalCreateBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
-        "Permissions": BackendStoragePermissionsTypeDef,
     },
     total=False,
 )
 
-class GetBackendStorageResourceConfigTypeDef(
-    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
+
+class CreateBackendStorageResourceConfigTypeDef(
+    _RequiredCreateBackendStorageResourceConfigTypeDef,
+    _OptionalCreateBackendStorageResourceConfigTypeDef,
 ):
     pass
 
+
 UpdateBackendStorageResourceConfigTypeDef = TypedDict(
     "UpdateBackendStorageResourceConfigTypeDef",
     {
         "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
@@ -1022,20 +1111,22 @@
     {
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateBackendAuthForgotPasswordConfigTypeDef(
     _RequiredCreateBackendAuthForgotPasswordConfigTypeDef,
     _OptionalCreateBackendAuthForgotPasswordConfigTypeDef,
 ):
     pass
 
+
 _RequiredCreateBackendAuthVerificationMessageConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthVerificationMessageConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
     },
 )
 _OptionalCreateBackendAuthVerificationMessageConfigTypeDef = TypedDict(
@@ -1043,20 +1134,22 @@
     {
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredCreateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalCreateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
+
 UpdateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
@@ -1074,39 +1167,65 @@
     {
         "EmailSettings": EmailSettingsTypeDef,
         "SmsSettings": SmsSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredUpdateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalUpdateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
+
+_RequiredCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "MFAMode": MFAModeType,
+    },
+)
+_OptionalCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "Settings": SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthMFAConfigOutputTypeDef(
+    _RequiredCreateBackendAuthMFAConfigOutputTypeDef,
+    _OptionalCreateBackendAuthMFAConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
     },
 )
 _OptionalCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_OptionalCreateBackendAuthMFAConfigTypeDef",
     {
         "Settings": SettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateBackendAuthMFAConfigTypeDef(
     _RequiredCreateBackendAuthMFAConfigTypeDef, _OptionalCreateBackendAuthMFAConfigTypeDef
 ):
     pass
 
+
 UpdateBackendAuthMFAConfigTypeDef = TypedDict(
     "UpdateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
         "Settings": SettingsTypeDef,
     },
     total=False,
@@ -1126,20 +1245,22 @@
         "Operation": str,
         "Status": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListBackendJobsRequestListBackendJobsPaginateTypeDef(
     _RequiredListBackendJobsRequestListBackendJobsPaginateTypeDef,
     _OptionalListBackendJobsRequestListBackendJobsPaginateTypeDef,
 ):
     pass
 
+
 ListS3BucketsResponseTypeDef = TypedDict(
     "ListS3BucketsResponseTypeDef",
     {
         "Buckets": List[S3BucketInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1155,44 +1276,85 @@
     "_OptionalUpdateBackendConfigRequestRequestTypeDef",
     {
         "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBackendConfigRequestRequestTypeDef(
     _RequiredUpdateBackendConfigRequestRequestTypeDef,
     _OptionalUpdateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateBackendConfigResponseTypeDef = TypedDict(
     "UpdateBackendConfigResponseTypeDef",
     {
         "AppId": str,
         "BackendManagerAppId": str,
         "Error": str,
         "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BackendAPIResourceConfigOutputTypeDef = TypedDict(
+    "BackendAPIResourceConfigOutputTypeDef",
+    {
+        "AdditionalAuthTypes": List[BackendAPIAuthTypeTypeDef],
+        "ApiName": str,
+        "ConflictResolution": BackendAPIConflictResolutionTypeDef,
+        "DefaultAuthType": BackendAPIAuthTypeTypeDef,
+        "Service": str,
+        "TransformSchema": str,
+    },
+    total=False,
+)
+
 BackendAPIResourceConfigTypeDef = TypedDict(
     "BackendAPIResourceConfigTypeDef",
     {
         "AdditionalAuthTypes": Sequence[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
         "ConflictResolution": BackendAPIConflictResolutionTypeDef,
         "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "OAuthGrantType": OAuthGrantTypeType,
+        "OAuthScopes": List[OAuthScopesElementType],
+        "RedirectSignInURIs": List[str],
+        "RedirectSignOutURIs": List[str],
+    },
+)
+_OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "DomainPrefix": str,
+        "SocialProviderSettings": SocialProviderSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthOAuthConfigOutputTypeDef(
+    _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
+    _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthOAuthConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthOAuthConfigTypeDef",
     {
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
@@ -1203,63 +1365,80 @@
     {
         "DomainPrefix": str,
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateBackendAuthOAuthConfigTypeDef(
     _RequiredCreateBackendAuthOAuthConfigTypeDef, _OptionalCreateBackendAuthOAuthConfigTypeDef
 ):
     pass
 
+
 UpdateBackendAuthOAuthConfigTypeDef = TypedDict(
     "UpdateBackendAuthOAuthConfigTypeDef",
     {
         "DomainPrefix": str,
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-CreateBackendStorageRequestRequestTypeDef = TypedDict(
-    "CreateBackendStorageRequestRequestTypeDef",
+GetBackendStorageResponseTypeDef = TypedDict(
+    "GetBackendStorageResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendStorageResponseTypeDef = TypedDict(
-    "GetBackendStorageResponseTypeDef",
+CreateBackendStorageRequestRequestTypeDef = TypedDict(
+    "CreateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBackendStorageRequestRequestTypeDef = TypedDict(
     "UpdateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
+GetBackendAPIResponseTypeDef = TypedDict(
+    "GetBackendAPIResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendEnvironmentName": str,
+        "Error": str,
+        "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BackendAPIResourceConfigUnionTypeDef = Union[
+    BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+]
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1278,19 +1457,21 @@
     "_OptionalDeleteBackendAPIRequestRequestTypeDef",
     {
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
     },
     total=False,
 )
 
+
 class DeleteBackendAPIRequestRequestTypeDef(
     _RequiredDeleteBackendAPIRequestRequestTypeDef, _OptionalDeleteBackendAPIRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredGetBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1299,30 +1480,20 @@
     "_OptionalGetBackendAPIRequestRequestTypeDef",
     {
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetBackendAPIRequestRequestTypeDef(
     _RequiredGetBackendAPIRequestRequestTypeDef, _OptionalGetBackendAPIRequestRequestTypeDef
 ):
     pass
 
-GetBackendAPIResponseTypeDef = TypedDict(
-    "GetBackendAPIResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": BackendAPIResourceConfigTypeDef,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredUpdateBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
@@ -1332,19 +1503,49 @@
     "_OptionalUpdateBackendAPIRequestRequestTypeDef",
     {
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBackendAPIRequestRequestTypeDef(
     _RequiredUpdateBackendAPIRequestRequestTypeDef, _OptionalUpdateBackendAPIRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "RequiredSignUpAttributes": List[RequiredSignUpAttributesElementType],
+        "SignInMethod": SignInMethodType,
+        "UserPoolName": str,
+    },
+)
+_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "ForgotPassword": CreateBackendAuthForgotPasswordConfigTypeDef,
+        "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
+        "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
+        "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+        "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthUserPoolConfigOutputTypeDef(
+    _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
+    _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthUserPoolConfigTypeDef",
     {
         "RequiredSignUpAttributes": Sequence[RequiredSignUpAttributesElementType],
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
@@ -1357,31 +1558,57 @@
         "OAuth": CreateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
+
 class CreateBackendAuthUserPoolConfigTypeDef(
     _RequiredCreateBackendAuthUserPoolConfigTypeDef, _OptionalCreateBackendAuthUserPoolConfigTypeDef
 ):
     pass
 
+
 UpdateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "UpdateBackendAuthUserPoolConfigTypeDef",
     {
         "ForgotPassword": UpdateBackendAuthForgotPasswordConfigTypeDef,
         "Mfa": UpdateBackendAuthMFAConfigTypeDef,
         "OAuth": UpdateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": UpdateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": UpdateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "AuthResources": AuthResourcesType,
+        "Service": Literal["COGNITO"],
+        "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
+    },
+)
+_OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthResourceConfigOutputTypeDef(
+    _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
+    _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1390,19 +1617,21 @@
     "_OptionalCreateBackendAuthResourceConfigTypeDef",
     {
         "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
     },
     total=False,
 )
 
+
 class CreateBackendAuthResourceConfigTypeDef(
     _RequiredCreateBackendAuthResourceConfigTypeDef, _OptionalCreateBackendAuthResourceConfigTypeDef
 ):
     pass
 
+
 _RequiredUpdateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredUpdateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": UpdateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1411,41 +1640,46 @@
     "_OptionalUpdateBackendAuthResourceConfigTypeDef",
     {
         "IdentityPoolConfigs": UpdateBackendAuthIdentityPoolConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBackendAuthResourceConfigTypeDef(
     _RequiredUpdateBackendAuthResourceConfigTypeDef, _OptionalUpdateBackendAuthResourceConfigTypeDef
 ):
     pass
 
-CreateBackendAuthRequestRequestTypeDef = TypedDict(
-    "CreateBackendAuthRequestRequestTypeDef",
+
+GetBackendAuthResponseTypeDef = TypedDict(
+    "GetBackendAuthResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
+        "Error": str,
+        "ResourceConfig": CreateBackendAuthResourceConfigOutputTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendAuthResponseTypeDef = TypedDict(
-    "GetBackendAuthResponseTypeDef",
+CreateBackendAuthRequestRequestTypeDef = TypedDict(
+    "CreateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateBackendAuthResourceConfigUnionTypeDef = Union[
+    CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
+]
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/PKG-INFO` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifybackend
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AmplifyBackend 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AmplifyBackend 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore amplifybackend type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amplifybackend"></a>
 
 # types-aiobotocore-amplifybackend
 
 [![PyPI - types-aiobotocore-amplifybackend](https://img.shields.io/pypi/v/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplifybackend?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplifybackend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifybackend)](https://pepy.tech/project/types-aiobotocore-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AmplifyBackend 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [types-aiobotocore-amplifybackend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/).
 
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
@@ -323,35 +322,38 @@
 )
 
 
 def check_value(value: AdditionalConstraintsElementType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplifybackend.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplifybackend.type_defs import (
     BackendAPIAppSyncAuthSettingsTypeDef,
     BackendAPIConflictResolutionTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
+    BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
+    CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
     CreateTokenRequestRequestTypeDef,
     DeleteBackendAuthRequestRequestTypeDef,
     DeleteBackendRequestRequestTypeDef,
     DeleteBackendStorageRequestRequestTypeDef,
@@ -373,16 +375,16 @@
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
     BackendAPIAuthTypeTypeDef,
     SocialProviderSettingsTypeDef,
-    CreateBackendStorageResourceConfigTypeDef,
     GetBackendStorageResourceConfigTypeDef,
+    CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResponseTypeDef,
@@ -406,42 +408,49 @@
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
+    CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
     UpdateBackendConfigRequestRequestTypeDef,
     UpdateBackendConfigResponseTypeDef,
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
+    CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
-    CreateBackendStorageRequestRequestTypeDef,
     GetBackendStorageResponseTypeDef,
+    CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
+    GetBackendAPIResponseTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
-    GetBackendAPIResponseTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
+    CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
-    CreateBackendAuthRequestRequestTypeDef,
     GetBackendAuthResponseTypeDef,
+    CreateBackendAuthRequestRequestTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_value() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt` & `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-cognito-identity-2.5.2.tar.gz` & `tmp/types-aiobotocore-cognito-identity-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-identity-2.5.2.tar", last modified: Sat Jul  8 01:43:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-identity-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
```

## Comparing `types-aiobotocore-cognito-identity-2.5.2.tar` & `types-aiobotocore-cognito-identity-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.121913 types-aiobotocore-cognito-identity-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-07-08 01:43:26.117913 types-aiobotocore-cognito-identity-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:26.121913 types-aiobotocore-cognito-identity-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.113912 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21136 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:44.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.117913 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.989618 types-aiobotocore-cognito-identity-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-08-02 14:52:04.981618 types-aiobotocore-cognito-identity-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.989618 types-aiobotocore-cognito-identity-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.981618 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19132 2023-08-02 14:35:19.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-08-02 14:35:19.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.981618 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/LICENSE` & `types-aiobotocore-cognito-identity-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2/PKG-INFO` & `types-aiobotocore-cognito-identity-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cognito-identity type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cognito-identity"></a>
 
 # types-aiobotocore-cognito-identity
 
 [![PyPI - types-aiobotocore-cognito-identity](https://img.shields.io/pypi/v/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-identity?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CognitoIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
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
@@ -311,77 +310,80 @@
 )
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cognito_identity.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
-    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
-    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    IdentityPoolTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
+    GetIdResponseTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
+    GetOpenIdTokenResponseTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseTypeDef,
+    IdentityPoolTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
+    RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
+    RoleMappingUnionTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/README.md` & `types-aiobotocore-cognito-identity-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cognito-identity"></a>
 
 # types-aiobotocore-cognito-identity
 
 [![PyPI - types-aiobotocore-cognito-identity](https://img.shields.io/pypi/v/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-identity?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CognitoIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
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
@@ -278,77 +278,80 @@
 )
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cognito_identity.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
-    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
-    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    IdentityPoolTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
+    GetIdResponseTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
+    GetOpenIdTokenResponseTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseTypeDef,
+    IdentityPoolTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
+    RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
+    RoleMappingUnionTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/setup.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-identity",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with"
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
-    keywords="aiobotocore cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cognito-identity type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cognito_identity": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/"
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/__init__.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/__init__.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/__main__.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoIdentity 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CognitoIdentity 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
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

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/client.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     GetIdResponseTypeDef,
     GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
+    IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
-    RoleMappingTypeDef,
+    RoleMappingUnionTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -141,17 +141,15 @@
         """
         Deletes an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.delete_identity_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#delete_identity_pool)
         """
 
-    async def describe_identity(
-        self, *, IdentityId: str
-    ) -> IdentityDescriptionResponseMetadataTypeDef:
+    async def describe_identity(self, *, IdentityId: str) -> IdentityDescriptionResponseTypeDef:
         """
         Returns metadata related to the given identity, including when the identity was
         created and any associated linked logins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.describe_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#describe_identity)
         """
@@ -317,15 +315,15 @@
         """
 
     async def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...
+        RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#set_identity_pool_roles)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/client.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     GetIdResponseTypeDef,
     GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
+    IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
-    RoleMappingTypeDef,
+    RoleMappingUnionTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -131,17 +131,15 @@
     async def delete_identity_pool(self, *, IdentityPoolId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.delete_identity_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#delete_identity_pool)
         """
-    async def describe_identity(
-        self, *, IdentityId: str
-    ) -> IdentityDescriptionResponseMetadataTypeDef:
+    async def describe_identity(self, *, IdentityId: str) -> IdentityDescriptionResponseTypeDef:
         """
         Returns metadata related to the given identity, including when the identity was
         created and any associated linked logins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.describe_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#describe_identity)
         """
@@ -293,15 +291,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#merge_developer_identities)
         """
     async def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...
+        RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#set_identity_pool_roles)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/literals.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/literals.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/paginator.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListIdentityPoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/paginators/#listidentitypoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/paginators/#listidentitypoolspaginator)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/paginator.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListIdentityPoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/paginators/#listidentitypoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/paginators/#listidentitypoolspaginator)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/type_defs.py` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,84 +4,86 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
-    data: CognitoIdentityProviderTypeDef = {...}
+    data: CognitoIdentityProviderTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AmbiguousRoleResolutionTypeType,
     ErrorCodeType,
     MappingRuleMatchTypeType,
     RoleMappingTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityInputRequestTypeDef",
     "GetIdInputRequestTypeDef",
-    "GetIdResponseTypeDef",
     "GetIdentityPoolRolesInputRequestTypeDef",
     "GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef",
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     "GetOpenIdTokenInputRequestTypeDef",
-    "GetOpenIdTokenResponseTypeDef",
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityDescriptionTypeDef",
     "IdentityPoolShortDescriptionTypeDef",
     "ListIdentitiesInputRequestTypeDef",
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
-    "LookupDeveloperIdentityResponseTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
-    "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
-    "IdentityPoolTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityResponseTypeDef",
+    "GetIdResponseTypeDef",
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    "GetOpenIdTokenResponseTypeDef",
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    "IdentityDescriptionResponseTypeDef",
+    "IdentityPoolTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "LookupDeveloperIdentityResponseTypeDef",
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    "SetPrincipalTagAttributeMapResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
+    "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
+    "RoleMappingUnionTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
@@ -105,14 +107,25 @@
 DeleteIdentitiesInputRequestTypeDef = TypedDict(
     "DeleteIdentitiesInputRequestTypeDef",
     {
         "IdentityIdsToDelete": Sequence[str],
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
 UnprocessedIdentityIdTypeDef = TypedDict(
     "UnprocessedIdentityIdTypeDef",
     {
         "IdentityId": str,
         "ErrorCode": ErrorCodeType,
     },
     total=False,
@@ -135,21 +148,14 @@
 DescribeIdentityPoolInputRequestTypeDef = TypedDict(
     "DescribeIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
     "_RequiredGetCredentialsForIdentityInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
@@ -157,22 +163,20 @@
     {
         "Logins": Mapping[str, str],
         "CustomRoleArn": str,
     },
     total=False,
 )
 
-
 class GetCredentialsForIdentityInputRequestTypeDef(
     _RequiredGetCredentialsForIdentityInputRequestTypeDef,
     _OptionalGetCredentialsForIdentityInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetIdInputRequestTypeDef = TypedDict(
     "_RequiredGetIdInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalGetIdInputRequestTypeDef = TypedDict(
@@ -180,29 +184,19 @@
     {
         "AccountId": str,
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
-
-GetIdResponseTypeDef = TypedDict(
-    "GetIdResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -219,91 +213,47 @@
         "IdentityId": str,
         "PrincipalTags": Mapping[str, str],
         "TokenDuration": int,
     },
     total=False,
 )
 
-
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-
-GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_OptionalGetOpenIdTokenInputRequestTypeDef",
     {
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
-
-GetOpenIdTokenResponseTypeDef = TypedDict(
-    "GetOpenIdTokenResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
 
-GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IdentityDescriptionResponseMetadataTypeDef = TypedDict(
-    "IdentityDescriptionResponseMetadataTypeDef",
-    {
-        "IdentityId": str,
-        "Logins": List[str],
-        "CreationDate": datetime,
-        "LastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityDescriptionTypeDef = TypedDict(
     "IdentityDescriptionTypeDef",
     {
         "IdentityId": str,
         "Logins": List[str],
         "CreationDate": datetime,
         "LastModifiedDate": datetime,
@@ -332,25 +282,25 @@
     {
         "NextToken": str,
         "HideDisabled": bool,
     },
     total=False,
 )
 
-
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
-
-ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
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
 
 _RequiredListIdentityPoolsInputRequestTypeDef = TypedDict(
     "_RequiredListIdentityPoolsInputRequestTypeDef",
     {
@@ -361,36 +311,26 @@
     "_OptionalListIdentityPoolsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityPoolsInputRequestTypeDef(
     _RequiredListIdentityPoolsInputRequestTypeDef, _OptionalListIdentityPoolsInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
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
 _RequiredLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
     "_RequiredLookupDeveloperIdentityInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
@@ -400,32 +340,20 @@
         "DeveloperUserIdentifier": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-
-LookupDeveloperIdentityResponseTypeDef = TypedDict(
-    "LookupDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "DeveloperUserIdentifierList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -438,43 +366,14 @@
         "SourceUserIdentifier": str,
         "DestinationUserIdentifier": str,
         "DeveloperProviderName": str,
         "IdentityPoolId": str,
     },
 )
 
-MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "_RequiredSetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -483,33 +382,20 @@
     {
         "UseDefaults": bool,
         "PrincipalTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
-
-SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "SetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -558,21 +444,19 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateIdentityPoolInputRequestTypeDef(
     _RequiredCreateIdentityPoolInputRequestTypeDef, _OptionalCreateIdentityPoolInputRequestTypeDef
 ):
     pass
 
-
 _RequiredIdentityPoolRequestTypeDef = TypedDict(
     "_RequiredIdentityPoolRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
@@ -587,81 +471,206 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCredentialsForIdentityResponseTypeDef = TypedDict(
+    "GetCredentialsForIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Credentials": CredentialsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIdResponseTypeDef = TypedDict(
+    "GetIdResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenResponseTypeDef = TypedDict(
+    "GetOpenIdTokenResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IdentityDescriptionResponseTypeDef = TypedDict(
+    "IdentityDescriptionResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Logins": List[str],
+        "CreationDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 IdentityPoolTypeDef = TypedDict(
     "IdentityPoolTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
         "AllowClassicFlow": bool,
         "SupportedLoginProviders": Dict[str, str],
         "DeveloperProviderName": str,
         "OpenIdConnectProviderARNs": List[str],
         "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": List[str],
         "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCredentialsForIdentityResponseTypeDef = TypedDict(
-    "GetCredentialsForIdentityResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LookupDeveloperIdentityResponseTypeDef = TypedDict(
+    "LookupDeveloperIdentityResponseTypeDef",
     {
         "IdentityId": str,
-        "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeveloperUserIdentifierList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "SetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIdentitiesResponseTypeDef = TypedDict(
     "DeleteIdentitiesResponseTypeDef",
     {
         "UnprocessedIdentityIds": List[UnprocessedIdentityIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentitiesResponseTypeDef = TypedDict(
     "ListIdentitiesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Identities": List[IdentityDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityPoolsResponseTypeDef = TypedDict(
     "ListIdentityPoolsResponseTypeDef",
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+RulesConfigurationTypeOutputTypeDef = TypedDict(
+    "RulesConfigurationTypeOutputTypeDef",
+    {
+        "Rules": List[MappingRuleTypeDef],
     },
 )
 
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
-        "Rules": List[MappingRuleTypeDef],
+        "Rules": Sequence[MappingRuleTypeDef],
     },
 )
 
+_RequiredRoleMappingOutputTypeDef = TypedDict(
+    "_RequiredRoleMappingOutputTypeDef",
+    {
+        "Type": RoleMappingTypeType,
+    },
+)
+_OptionalRoleMappingOutputTypeDef = TypedDict(
+    "_OptionalRoleMappingOutputTypeDef",
+    {
+        "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
+        "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
+    },
+    total=False,
+)
+
+class RoleMappingOutputTypeDef(
+    _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
+):
+    pass
+
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
 _OptionalRoleMappingTypeDef = TypedDict(
@@ -669,43 +678,41 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class RoleMappingTypeDef(_RequiredRoleMappingTypeDef, _OptionalRoleMappingTypeDef):
     pass
 
-
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
-        "RoleMappings": Dict[str, RoleMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RoleMappingUnionTypeDef = Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Mapping[str, str],
     },
 )
 _OptionalSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
-        "RoleMappings": Mapping[str, RoleMappingTypeDef],
+        "RoleMappings": Mapping[str, RoleMappingUnionTypeDef],
     },
     total=False,
 )
 
-
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity/type_defs.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,83 +4,87 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
-    data: CognitoIdentityProviderTypeDef = {...}
+    data: CognitoIdentityProviderTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AmbiguousRoleResolutionTypeType,
     ErrorCodeType,
     MappingRuleMatchTypeType,
     RoleMappingTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityInputRequestTypeDef",
     "GetIdInputRequestTypeDef",
-    "GetIdResponseTypeDef",
     "GetIdentityPoolRolesInputRequestTypeDef",
     "GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef",
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     "GetOpenIdTokenInputRequestTypeDef",
-    "GetOpenIdTokenResponseTypeDef",
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityDescriptionTypeDef",
     "IdentityPoolShortDescriptionTypeDef",
     "ListIdentitiesInputRequestTypeDef",
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
-    "LookupDeveloperIdentityResponseTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
-    "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
-    "IdentityPoolTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityResponseTypeDef",
+    "GetIdResponseTypeDef",
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    "GetOpenIdTokenResponseTypeDef",
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    "IdentityDescriptionResponseTypeDef",
+    "IdentityPoolTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "LookupDeveloperIdentityResponseTypeDef",
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    "SetPrincipalTagAttributeMapResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
+    "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
+    "RoleMappingUnionTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
@@ -104,14 +108,25 @@
 DeleteIdentitiesInputRequestTypeDef = TypedDict(
     "DeleteIdentitiesInputRequestTypeDef",
     {
         "IdentityIdsToDelete": Sequence[str],
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
 UnprocessedIdentityIdTypeDef = TypedDict(
     "UnprocessedIdentityIdTypeDef",
     {
         "IdentityId": str,
         "ErrorCode": ErrorCodeType,
     },
     total=False,
@@ -134,21 +149,14 @@
 DescribeIdentityPoolInputRequestTypeDef = TypedDict(
     "DescribeIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
     "_RequiredGetCredentialsForIdentityInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
@@ -156,20 +164,22 @@
     {
         "Logins": Mapping[str, str],
         "CustomRoleArn": str,
     },
     total=False,
 )
 
+
 class GetCredentialsForIdentityInputRequestTypeDef(
     _RequiredGetCredentialsForIdentityInputRequestTypeDef,
     _OptionalGetCredentialsForIdentityInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetIdInputRequestTypeDef = TypedDict(
     "_RequiredGetIdInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalGetIdInputRequestTypeDef = TypedDict(
@@ -177,26 +187,20 @@
     {
         "AccountId": str,
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
-GetIdResponseTypeDef = TypedDict(
-    "GetIdResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
@@ -214,28 +218,21 @@
         "IdentityId": str,
         "PrincipalTags": Mapping[str, str],
         "TokenDuration": int,
     },
     total=False,
 )
 
+
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
@@ -243,58 +240,29 @@
     "_OptionalGetOpenIdTokenInputRequestTypeDef",
     {
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
-GetOpenIdTokenResponseTypeDef = TypedDict(
-    "GetOpenIdTokenResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
 
-GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IdentityDescriptionResponseMetadataTypeDef = TypedDict(
-    "IdentityDescriptionResponseMetadataTypeDef",
-    {
-        "IdentityId": str,
-        "Logins": List[str],
-        "CreationDate": datetime,
-        "LastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityDescriptionTypeDef = TypedDict(
     "IdentityDescriptionTypeDef",
     {
         "IdentityId": str,
         "Logins": List[str],
         "CreationDate": datetime,
         "LastModifiedDate": datetime,
@@ -323,23 +291,27 @@
     {
         "NextToken": str,
         "HideDisabled": bool,
     },
     total=False,
 )
 
+
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
-ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+
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
 
 _RequiredListIdentityPoolsInputRequestTypeDef = TypedDict(
     "_RequiredListIdentityPoolsInputRequestTypeDef",
     {
@@ -350,34 +322,28 @@
     "_OptionalListIdentityPoolsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityPoolsInputRequestTypeDef(
     _RequiredListIdentityPoolsInputRequestTypeDef, _OptionalListIdentityPoolsInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
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
 _RequiredLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
     "_RequiredLookupDeveloperIdentityInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
@@ -387,29 +353,21 @@
         "DeveloperUserIdentifier": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-LookupDeveloperIdentityResponseTypeDef = TypedDict(
-    "LookupDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "DeveloperUserIdentifierList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
@@ -423,43 +381,14 @@
         "SourceUserIdentifier": str,
         "DestinationUserIdentifier": str,
         "DeveloperProviderName": str,
         "IdentityPoolId": str,
     },
 )
 
-MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "_RequiredSetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -468,30 +397,21 @@
     {
         "UseDefaults": bool,
         "PrincipalTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
-SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "SetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
@@ -541,19 +461,21 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateIdentityPoolInputRequestTypeDef(
     _RequiredCreateIdentityPoolInputRequestTypeDef, _OptionalCreateIdentityPoolInputRequestTypeDef
 ):
     pass
 
+
 _RequiredIdentityPoolRequestTypeDef = TypedDict(
     "_RequiredIdentityPoolRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
@@ -568,78 +490,209 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCredentialsForIdentityResponseTypeDef = TypedDict(
+    "GetCredentialsForIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Credentials": CredentialsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIdResponseTypeDef = TypedDict(
+    "GetIdResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenResponseTypeDef = TypedDict(
+    "GetOpenIdTokenResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IdentityDescriptionResponseTypeDef = TypedDict(
+    "IdentityDescriptionResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Logins": List[str],
+        "CreationDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 IdentityPoolTypeDef = TypedDict(
     "IdentityPoolTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
         "AllowClassicFlow": bool,
         "SupportedLoginProviders": Dict[str, str],
         "DeveloperProviderName": str,
         "OpenIdConnectProviderARNs": List[str],
         "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": List[str],
         "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCredentialsForIdentityResponseTypeDef = TypedDict(
-    "GetCredentialsForIdentityResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LookupDeveloperIdentityResponseTypeDef = TypedDict(
+    "LookupDeveloperIdentityResponseTypeDef",
     {
         "IdentityId": str,
-        "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeveloperUserIdentifierList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "SetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIdentitiesResponseTypeDef = TypedDict(
     "DeleteIdentitiesResponseTypeDef",
     {
         "UnprocessedIdentityIds": List[UnprocessedIdentityIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentitiesResponseTypeDef = TypedDict(
     "ListIdentitiesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Identities": List[IdentityDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityPoolsResponseTypeDef = TypedDict(
     "ListIdentityPoolsResponseTypeDef",
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+RulesConfigurationTypeOutputTypeDef = TypedDict(
+    "RulesConfigurationTypeOutputTypeDef",
+    {
+        "Rules": List[MappingRuleTypeDef],
     },
 )
 
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
-        "Rules": List[MappingRuleTypeDef],
+        "Rules": Sequence[MappingRuleTypeDef],
+    },
+)
+
+_RequiredRoleMappingOutputTypeDef = TypedDict(
+    "_RequiredRoleMappingOutputTypeDef",
+    {
+        "Type": RoleMappingTypeType,
     },
 )
+_OptionalRoleMappingOutputTypeDef = TypedDict(
+    "_OptionalRoleMappingOutputTypeDef",
+    {
+        "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
+        "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RoleMappingOutputTypeDef(
+    _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
+):
+    pass
+
 
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
@@ -648,40 +701,44 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class RoleMappingTypeDef(_RequiredRoleMappingTypeDef, _OptionalRoleMappingTypeDef):
     pass
 
+
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
-        "RoleMappings": Dict[str, RoleMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RoleMappingUnionTypeDef = Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Mapping[str, str],
     },
 )
 _OptionalSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
-        "RoleMappings": Mapping[str, RoleMappingTypeDef],
+        "RoleMappings": Mapping[str, RoleMappingUnionTypeDef],
     },
     total=False,
 )
 
+
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/PKG-INFO` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cognito-identity type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cognito-identity"></a>
 
 # types-aiobotocore-cognito-identity
 
 [![PyPI - types-aiobotocore-cognito-identity](https://img.shields.io/pypi/v/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-identity?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CognitoIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
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
@@ -311,77 +310,80 @@
 )
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cognito_identity.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
-    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
-    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    IdentityPoolTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
+    GetIdResponseTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
+    GetOpenIdTokenResponseTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseTypeDef,
+    IdentityPoolTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
+    RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
+    RoleMappingUnionTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*


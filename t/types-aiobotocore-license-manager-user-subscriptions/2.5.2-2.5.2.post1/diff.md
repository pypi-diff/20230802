# Comparing `tmp/types-aiobotocore-license-manager-user-subscriptions-2.5.2.tar.gz` & `tmp/types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-user-subscriptions-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:34 2023, max compression
```

## Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.tar` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.770435 types-aiobotocore-license-manager-user-subscriptions-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:04.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-08 01:43:53.770435 types-aiobotocore-license-manager-user-subscriptions-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-08 01:34:04.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.774435 types-aiobotocore-license-manager-user-subscriptions-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-08 01:34:04.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.770435 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-08 01:34:04.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-08 01:34:04.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-08 01:34:05.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-08 01:34:05.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-07-08 01:34:05.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-08 01:34:06.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-08 01:34:06.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-08 01:34:05.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-08 01:34:05.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:05.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15879 2023-07-08 01:34:06.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-08 01:34:06.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:04.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.770435 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16537 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-08-02 14:42:17.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16537 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/LICENSE` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/PKG-INFO` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-user-subscriptions
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore license-manager-user-subscriptions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/types-aiobotocore-license-manager-user-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager-user-subscriptions)](https://pepy.tech/project/types-aiobotocore-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LicenseManagerUserSubscriptions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
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
@@ -330,37 +329,39 @@
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_license_manager_user_subscriptions.type_defs` module
-contains structures and shapes assembled to typed dictionaries for additional
-type checking.
+contains structures and shapes assembled to typed dictionaries and unions for
+additional type checking.
 
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
-    SettingsTypeDef,
+    SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListIdentityProvidersRequestRequestTypeDef,
+    SettingsTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
+    SettingsUnionTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -380,15 +381,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/README.md` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/types-aiobotocore-license-manager-user-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager-user-subscriptions)](https://pepy.tech/project/types-aiobotocore-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LicenseManagerUserSubscriptions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
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
@@ -297,37 +297,39 @@
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_license_manager_user_subscriptions.type_defs` module
-contains structures and shapes assembled to typed dictionaries for additional
-type checking.
+contains structures and shapes assembled to typed dictionaries and unions for
+additional type checking.
 
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
-    SettingsTypeDef,
+    SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListIdentityProvidersRequestRequestTypeDef,
+    SettingsTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
+    SettingsUnionTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -347,15 +349,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/setup.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager-user-subscriptions",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated"
-        " with mypy-boto3-builder 7.14.5"
+        " with mypy-boto3-builder 7.17.1"
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
-        "aiobotocore license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed"
+        "aiobotocore license-manager-user-subscriptions type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_license_manager_user_subscriptions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/__init__.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/__main__.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/client.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
-    SettingsTypeDef,
+    SettingsUnionTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -212,15 +212,15 @@
         """
 
     async def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsTypeDef = ...
+        Settings: SettingsUnionTypeDef = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/client.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
-    SettingsTypeDef,
+    SettingsUnionTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -197,15 +197,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#list_user_associations)
         """
     async def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsTypeDef = ...
+        Settings: SettingsUnionTypeDef = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/literals.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/literals.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/paginator.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 class ListIdentityProvidersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
         """
 
 
@@ -80,15 +80,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
 
@@ -100,15 +100,15 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
 
@@ -120,13 +120,13 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class ListIdentityProvidersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
         """
 
 class ListInstancesPaginator(AioPaginator):
@@ -76,15 +76,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
 class ListProductSubscriptionsPaginator(AioPaginator):
@@ -95,15 +95,15 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
 class ListUserAssociationsPaginator(AioPaginator):
@@ -114,13 +114,13 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/type_defs.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
-    data: ActiveDirectoryIdentityProviderTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
-    "SettingsTypeDef",
+    "SettingsOutputTypeDef",
     "InstanceSummaryTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListIdentityProvidersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListIdentityProvidersRequestRequestTypeDef",
+    "SettingsTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "SettingsUnionTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -64,26 +65,37 @@
     "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
     total=False,
 )
 
-SettingsTypeDef = TypedDict(
-    "SettingsTypeDef",
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": List[str],
     },
 )
 
 _RequiredInstanceSummaryTypeDef = TypedDict(
@@ -99,54 +111,41 @@
     {
         "LastStatusCheckDate": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
-
-ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
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
 
 ListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "ListIdentityProvidersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SettingsTypeDef = TypedDict(
+    "SettingsTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SecurityGroupId": str,
+        "Subnets": Sequence[str],
     },
 )
 
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
@@ -157,36 +156,25 @@
     "_OptionalUpdateSettingsTypeDef",
     {
         "SecurityGroupId": str,
     },
     total=False,
 )
 
-
 class UpdateSettingsTypeDef(_RequiredUpdateSettingsTypeDef, _OptionalUpdateSettingsTypeDef):
     pass
 
-
 IdentityProviderTypeDef = TypedDict(
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
 
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -194,18 +182,36 @@
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
+SettingsUnionTypeDef = Union[SettingsTypeDef, SettingsOutputTypeDef]
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
@@ -214,21 +220,19 @@
     "_OptionalAssociateUserRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-
 class AssociateUserRequestRequestTypeDef(
     _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
 ):
     pass
 
-
 DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "DeregisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -245,45 +249,41 @@
     "_OptionalDisassociateUserRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-
 class DisassociateUserRequestRequestTypeDef(
     _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredIdentityProviderSummaryTypeDef = TypedDict(
     "_RequiredIdentityProviderSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
-        "Settings": SettingsTypeDef,
+        "Settings": SettingsOutputTypeDef,
         "Status": str,
     },
 )
 _OptionalIdentityProviderSummaryTypeDef = TypedDict(
     "_OptionalIdentityProviderSummaryTypeDef",
     {
         "FailureMessage": str,
     },
     total=False,
 )
 
-
 class IdentityProviderSummaryTypeDef(
     _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
 ):
     pass
 
-
 _RequiredInstanceUserSummaryTypeDef = TypedDict(
     "_RequiredInstanceUserSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Status": str,
         "Username": str,
@@ -296,45 +296,41 @@
         "DisassociationDate": str,
         "Domain": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-
 class InstanceUserSummaryTypeDef(
     _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
 ):
     pass
 
-
 _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
 _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListProductSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -344,46 +340,42 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProductSubscriptionsRequestRequestTypeDef(
     _RequiredListProductSubscriptionsRequestRequestTypeDef,
     _OptionalListProductSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
 _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUserAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
@@ -393,22 +385,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListUserAssociationsRequestRequestTypeDef(
     _RequiredListUserAssociationsRequestRequestTypeDef,
     _OptionalListUserAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredProductUserSummaryTypeDef = TypedDict(
     "_RequiredProductUserSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Status": str,
         "Username": str,
@@ -421,21 +411,19 @@
         "StatusMessage": str,
         "SubscriptionEndDate": str,
         "SubscriptionStartDate": str,
     },
     total=False,
 )
 
-
 class ProductUserSummaryTypeDef(
     _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
 ):
     pass
 
-
 _RequiredRegisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -443,22 +431,20 @@
     "_OptionalRegisterIdentityProviderRequestRequestTypeDef",
     {
         "Settings": SettingsTypeDef,
     },
     total=False,
 )
 
-
 class RegisterIdentityProviderRequestRequestTypeDef(
     _RequiredRegisterIdentityProviderRequestRequestTypeDef,
     _OptionalRegisterIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -467,22 +453,20 @@
     "_OptionalStartProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-
 class StartProductSubscriptionRequestRequestTypeDef(
     _RequiredStartProductSubscriptionRequestRequestTypeDef,
     _OptionalStartProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStopProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStopProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -491,106 +475,104 @@
     "_OptionalStopProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-
 class StopProductSubscriptionRequestRequestTypeDef(
     _RequiredStopProductSubscriptionRequestRequestTypeDef,
     _OptionalStopProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateIdentityProviderSettingsRequestRequestTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "UpdateSettings": UpdateSettingsTypeDef,
     },
 )
 
 DeregisterIdentityProviderResponseTypeDef = TypedDict(
     "DeregisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "IdentityProviderSummaries": List[IdentityProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterIdentityProviderResponseTypeDef = TypedDict(
     "RegisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderSettingsResponseTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateUserResponseTypeDef = TypedDict(
     "AssociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateUserResponseTypeDef = TypedDict(
     "DisassociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAssociationsResponseTypeDef = TypedDict(
     "ListUserAssociationsResponseTypeDef",
     {
         "InstanceUserSummaries": List[InstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProductSubscriptionsResponseTypeDef = TypedDict(
     "ListProductSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "ProductUserSummaries": List[ProductUserSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProductSubscriptionResponseTypeDef = TypedDict(
     "StartProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopProductSubscriptionResponseTypeDef = TypedDict(
     "StopProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
-    data: ActiveDirectoryIdentityProviderTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
-    "SettingsTypeDef",
+    "SettingsOutputTypeDef",
     "InstanceSummaryTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListIdentityProvidersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListIdentityProvidersRequestRequestTypeDef",
+    "SettingsTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "SettingsUnionTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -63,26 +66,37 @@
     "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
     total=False,
 )
 
-SettingsTypeDef = TypedDict(
-    "SettingsTypeDef",
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": List[str],
     },
 )
 
 _RequiredInstanceSummaryTypeDef = TypedDict(
@@ -98,52 +112,43 @@
     {
         "LastStatusCheckDate": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
-ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
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
 
 ListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "ListIdentityProvidersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SettingsTypeDef = TypedDict(
+    "SettingsTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SecurityGroupId": str,
+        "Subnets": Sequence[str],
     },
 )
 
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
@@ -154,34 +159,27 @@
     "_OptionalUpdateSettingsTypeDef",
     {
         "SecurityGroupId": str,
     },
     total=False,
 )
 
+
 class UpdateSettingsTypeDef(_RequiredUpdateSettingsTypeDef, _OptionalUpdateSettingsTypeDef):
     pass
 
+
 IdentityProviderTypeDef = TypedDict(
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
 
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -189,18 +187,36 @@
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
+SettingsUnionTypeDef = Union[SettingsTypeDef, SettingsOutputTypeDef]
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
@@ -209,19 +225,21 @@
     "_OptionalAssociateUserRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
+
 class AssociateUserRequestRequestTypeDef(
     _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
 ):
     pass
 
+
 DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "DeregisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -238,41 +256,45 @@
     "_OptionalDisassociateUserRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
+
 class DisassociateUserRequestRequestTypeDef(
     _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredIdentityProviderSummaryTypeDef = TypedDict(
     "_RequiredIdentityProviderSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
-        "Settings": SettingsTypeDef,
+        "Settings": SettingsOutputTypeDef,
         "Status": str,
     },
 )
 _OptionalIdentityProviderSummaryTypeDef = TypedDict(
     "_OptionalIdentityProviderSummaryTypeDef",
     {
         "FailureMessage": str,
     },
     total=False,
 )
 
+
 class IdentityProviderSummaryTypeDef(
     _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
 ):
     pass
 
+
 _RequiredInstanceUserSummaryTypeDef = TypedDict(
     "_RequiredInstanceUserSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Status": str,
         "Username": str,
@@ -285,41 +307,45 @@
         "DisassociationDate": str,
         "Domain": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+
 class InstanceUserSummaryTypeDef(
     _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
 ):
     pass
 
+
 _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
 _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListProductSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -329,42 +355,46 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProductSubscriptionsRequestRequestTypeDef(
     _RequiredListProductSubscriptionsRequestRequestTypeDef,
     _OptionalListProductSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
 _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUserAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
@@ -374,20 +404,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListUserAssociationsRequestRequestTypeDef(
     _RequiredListUserAssociationsRequestRequestTypeDef,
     _OptionalListUserAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredProductUserSummaryTypeDef = TypedDict(
     "_RequiredProductUserSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Status": str,
         "Username": str,
@@ -400,19 +432,21 @@
         "StatusMessage": str,
         "SubscriptionEndDate": str,
         "SubscriptionStartDate": str,
     },
     total=False,
 )
 
+
 class ProductUserSummaryTypeDef(
     _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
 ):
     pass
 
+
 _RequiredRegisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -420,20 +454,22 @@
     "_OptionalRegisterIdentityProviderRequestRequestTypeDef",
     {
         "Settings": SettingsTypeDef,
     },
     total=False,
 )
 
+
 class RegisterIdentityProviderRequestRequestTypeDef(
     _RequiredRegisterIdentityProviderRequestRequestTypeDef,
     _OptionalRegisterIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -442,20 +478,22 @@
     "_OptionalStartProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
+
 class StartProductSubscriptionRequestRequestTypeDef(
     _RequiredStartProductSubscriptionRequestRequestTypeDef,
     _OptionalStartProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStopProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStopProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -464,104 +502,106 @@
     "_OptionalStopProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
+
 class StopProductSubscriptionRequestRequestTypeDef(
     _RequiredStopProductSubscriptionRequestRequestTypeDef,
     _OptionalStopProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateIdentityProviderSettingsRequestRequestTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "UpdateSettings": UpdateSettingsTypeDef,
     },
 )
 
 DeregisterIdentityProviderResponseTypeDef = TypedDict(
     "DeregisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "IdentityProviderSummaries": List[IdentityProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterIdentityProviderResponseTypeDef = TypedDict(
     "RegisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderSettingsResponseTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateUserResponseTypeDef = TypedDict(
     "AssociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateUserResponseTypeDef = TypedDict(
     "DisassociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAssociationsResponseTypeDef = TypedDict(
     "ListUserAssociationsResponseTypeDef",
     {
         "InstanceUserSummaries": List[InstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProductSubscriptionsResponseTypeDef = TypedDict(
     "ListProductSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "ProductUserSummaries": List[ProductUserSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProductSubscriptionResponseTypeDef = TypedDict(
     "StartProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopProductSubscriptionResponseTypeDef = TypedDict(
     "StopProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-user-subscriptions
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore license-manager-user-subscriptions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/types-aiobotocore-license-manager-user-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager-user-subscriptions)](https://pepy.tech/project/types-aiobotocore-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LicenseManagerUserSubscriptions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
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
@@ -330,37 +329,39 @@
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_license_manager_user_subscriptions.type_defs` module
-contains structures and shapes assembled to typed dictionaries for additional
-type checking.
+contains structures and shapes assembled to typed dictionaries and unions for
+additional type checking.
 
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
-    SettingsTypeDef,
+    SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListIdentityProvidersRequestRequestTypeDef,
+    SettingsTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
+    SettingsUnionTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -380,15 +381,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


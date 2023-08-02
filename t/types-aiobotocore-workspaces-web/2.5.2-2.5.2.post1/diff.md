# Comparing `tmp/types-aiobotocore-workspaces-web-2.5.2.tar.gz` & `tmp/types-aiobotocore-workspaces-web-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-web-2.5.2.tar", last modified: Sat Jul  8 01:44:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-web-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
```

## Comparing `types-aiobotocore-workspaces-web-2.5.2.tar` & `types-aiobotocore-workspaces-web-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:29.355067 types-aiobotocore-workspaces-web-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-08 01:44:29.355067 types-aiobotocore-workspaces-web-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:29.355067 types-aiobotocore-workspaces-web-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:29.355067 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40444 2023-07-08 01:42:50.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40378 2023-07-08 01:42:50.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-08 01:42:50.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-08 01:42:50.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41413 2023-07-08 01:42:51.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41362 2023-07-08 01:42:50.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:49.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:29.355067 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-08 01:44:29.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-08 01:44:29.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:29.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:29.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:29.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:29.000000 types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:51:24.000000 types-aiobotocore-workspaces-web-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40343 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40277 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41342 2023-08-02 14:51:26.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41291 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/LICENSE` & `types-aiobotocore-workspaces-web-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2/PKG-INFO` & `types-aiobotocore-workspaces-web-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces-web
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore workspaces-web type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore workspaces-web type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-workspaces-web"></a>
 
 # types-aiobotocore-workspaces-web
 
 [![PyPI - types-aiobotocore-workspaces-web](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workspaces-web?color=blue)](https://pypistats.org/packages/types-aiobotocore-workspaces-web)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-web)](https://pepy.tech/project/types-aiobotocore-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkSpacesWeb 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [types-aiobotocore-workspaces-web docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/).
 
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
@@ -286,50 +285,38 @@
 )
 
 
 def check_value(value: AuthenticationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_workspaces_web.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
-    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
-    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
-    AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    CreateIdentityProviderResponseTypeDef,
     IpRuleTypeDef,
-    CreateIpAccessSettingsResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
@@ -345,15 +332,14 @@
     IdentityProviderTypeDef,
     GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
@@ -370,24 +356,38 @@
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
-    UpdateTrustStoreRequestRequestTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
+    AssociateTrustStoreResponseTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
+    AssociateUserSettingsResponseTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
+    UpdateTrustStoreResponseTypeDef,
+    UpdateTrustStoreRequestRequestTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
@@ -419,15 +419,15 @@
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
+def get_value() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/README.md` & `types-aiobotocore-workspaces-web-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-workspaces-web"></a>
 
 # types-aiobotocore-workspaces-web
 
 [![PyPI - types-aiobotocore-workspaces-web](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workspaces-web?color=blue)](https://pypistats.org/packages/types-aiobotocore-workspaces-web)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-web)](https://pepy.tech/project/types-aiobotocore-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkSpacesWeb 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [types-aiobotocore-workspaces-web docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/).
 
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
@@ -253,50 +253,38 @@
 )
 
 
 def check_value(value: AuthenticationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_workspaces_web.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
-    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
-    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
-    AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    CreateIdentityProviderResponseTypeDef,
     IpRuleTypeDef,
-    CreateIpAccessSettingsResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
@@ -312,15 +300,14 @@
     IdentityProviderTypeDef,
     GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
@@ -337,24 +324,38 @@
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
-    UpdateTrustStoreRequestRequestTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
+    AssociateTrustStoreResponseTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
+    AssociateUserSettingsResponseTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
+    UpdateTrustStoreResponseTypeDef,
+    UpdateTrustStoreRequestRequestTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
@@ -386,15 +387,15 @@
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
+def get_value() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/setup.py` & `types-aiobotocore-workspaces-web-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces-web",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkSpacesWeb 2.5.2 service generated with"
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
-    keywords="aiobotocore workspaces-web type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore workspaces-web type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workspaces_web": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/"
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/__main__.py` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkSpacesWeb 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WorkSpacesWeb 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
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

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/client.py` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
 
     session = get_session()
     async with session.create_client("workspaces-web") as client:
         client: WorkSpacesWebClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateIpAccessSettingsResponseTypeDef,
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
@@ -266,15 +266,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_portal)
         """
 
     async def create_trust_store(
         self,
         *,
-        certificateList: Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
@@ -724,15 +724,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_portal)
         """
 
     async def update_trust_store(
         self,
         *,
         trustStoreArn: str,
-        certificatesToAdd: Sequence[Union[str, bytes, IO[Any], StreamingBody]] = ...,
+        certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
         clientToken: str = ...
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/client.pyi` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
 
     session = get_session()
     async with session.create_client("workspaces-web") as client:
         client: WorkSpacesWebClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateIpAccessSettingsResponseTypeDef,
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
@@ -249,15 +249,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_portal)
         """
     async def create_trust_store(
         self,
         *,
-        certificateList: Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
@@ -662,15 +662,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_portal)
         """
     async def update_trust_store(
         self,
         *,
         trustStoreArn: str,
-        certificatesToAdd: Sequence[Union[str, bytes, IO[Any], StreamingBody]] = ...,
+        certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
         clientToken: str = ...
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/literals.py` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/literals.pyi` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/type_defs.py` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef
 
-    data: AssociateBrowserSettingsRequestRequestTypeDef = {...}
+    data: AssociateBrowserSettingsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -32,40 +32,28 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
-    "AssociateBrowserSettingsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
-    "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
-    "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
-    "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
-    "AssociateUserSettingsResponseTypeDef",
+    "BlobTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
-    "CreateBrowserSettingsResponseTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
     "IpRuleTypeDef",
-    "CreateIpAccessSettingsResponseTypeDef",
-    "CreateNetworkSettingsResponseTypeDef",
-    "CreatePortalResponseTypeDef",
-    "CreateTrustStoreResponseTypeDef",
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    "CreateUserSettingsResponseTypeDef",
     "DeleteBrowserSettingsRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
     "DeleteIpAccessSettingsRequestRequestTypeDef",
     "DeleteNetworkSettingsRequestRequestTypeDef",
     "DeletePortalRequestRequestTypeDef",
     "DeleteTrustStoreRequestRequestTypeDef",
     "DeleteUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -81,15 +69,14 @@
     "IdentityProviderTypeDef",
     "GetIpAccessSettingsRequestRequestTypeDef",
     "GetNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsTypeDef",
     "GetPortalRequestRequestTypeDef",
     "PortalTypeDef",
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
-    "GetPortalServiceProviderMetadataResponseTypeDef",
     "GetTrustStoreCertificateRequestRequestTypeDef",
     "GetTrustStoreRequestRequestTypeDef",
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
@@ -106,24 +93,38 @@
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
-    "UpdateTrustStoreRequestRequestTypeDef",
-    "UpdateTrustStoreResponseTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
+    "AssociateBrowserSettingsResponseTypeDef",
+    "AssociateIpAccessSettingsResponseTypeDef",
+    "AssociateNetworkSettingsResponseTypeDef",
+    "AssociateTrustStoreResponseTypeDef",
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    "AssociateUserSettingsResponseTypeDef",
+    "CreateBrowserSettingsResponseTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "CreateIpAccessSettingsResponseTypeDef",
+    "CreateNetworkSettingsResponseTypeDef",
+    "CreatePortalResponseTypeDef",
+    "CreateTrustStoreResponseTypeDef",
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    "CreateUserSettingsResponseTypeDef",
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    "UpdateTrustStoreResponseTypeDef",
+    "UpdateTrustStoreRequestRequestTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
@@ -162,108 +163,66 @@
     "AssociateBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateBrowserSettingsResponseTypeDef = TypedDict(
-    "AssociateBrowserSettingsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "browserSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateIpAccessSettingsResponseTypeDef = TypedDict(
-    "AssociateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "AssociateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateNetworkSettingsResponseTypeDef = TypedDict(
-    "AssociateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateTrustStoreRequestRequestTypeDef = TypedDict(
     "AssociateTrustStoreRequestRequestTypeDef",
     {
         "portalArn": str,
         "trustStoreArn": str,
     },
 )
 
-AssociateTrustStoreResponseTypeDef = TypedDict(
-    "AssociateTrustStoreResponseTypeDef",
-    {
-        "portalArn": str,
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userAccessLoggingSettingsArn": str,
     },
 )
 
-AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
-AssociateUserSettingsResponseTypeDef = TypedDict(
-    "AssociateUserSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -317,22 +276,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateBrowserSettingsResponseTypeDef = TypedDict(
-    "CreateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
         "portalArn": str,
@@ -350,22 +301,14 @@
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
-    {
-        "identityProviderArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIpRuleTypeDef = TypedDict(
     "_RequiredIpRuleTypeDef",
     {
         "ipRange": str,
     },
 )
 _OptionalIpRuleTypeDef = TypedDict(
@@ -377,63 +320,14 @@
 )
 
 
 class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
     pass
 
 
-CreateIpAccessSettingsResponseTypeDef = TypedDict(
-    "CreateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkSettingsResponseTypeDef = TypedDict(
-    "CreateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePortalResponseTypeDef = TypedDict(
-    "CreatePortalResponseTypeDef",
-    {
-        "portalArn": str,
-        "portalEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTrustStoreResponseTypeDef = TypedDict(
-    "CreateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserSettingsResponseTypeDef = TypedDict(
-    "CreateUserSettingsResponseTypeDef",
-    {
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
@@ -631,23 +525,14 @@
 GetPortalServiceProviderMetadataRequestRequestTypeDef = TypedDict(
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
-GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    {
-        "portalArn": str,
-        "serviceProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrustStoreCertificateRequestRequestTypeDef = TypedDict(
     "GetTrustStoreCertificateRequestRequestTypeDef",
     {
         "thumbprint": str,
         "trustStoreArn": str,
     },
 )
@@ -925,25 +810,14 @@
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
         "userSettingsArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1039,45 +913,14 @@
 
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "trustStoreArn": str,
-    },
-)
-_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-        "certificatesToDelete": Sequence[str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateTrustStoreRequestRequestTypeDef(
-    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
-):
-    pass
-
-
-UpdateTrustStoreResponseTypeDef = TypedDict(
-    "UpdateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1122,55 +965,214 @@
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateBrowserSettingsResponseTypeDef = TypedDict(
+    "AssociateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateIpAccessSettingsResponseTypeDef = TypedDict(
+    "AssociateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateNetworkSettingsResponseTypeDef = TypedDict(
+    "AssociateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateTrustStoreResponseTypeDef = TypedDict(
+    "AssociateTrustStoreResponseTypeDef",
+    {
+        "portalArn": str,
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserSettingsResponseTypeDef = TypedDict(
+    "AssociateUserSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBrowserSettingsResponseTypeDef = TypedDict(
+    "CreateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
+    {
+        "identityProviderArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIpAccessSettingsResponseTypeDef = TypedDict(
+    "CreateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkSettingsResponseTypeDef = TypedDict(
+    "CreateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortalResponseTypeDef = TypedDict(
+    "CreatePortalResponseTypeDef",
+    {
+        "portalArn": str,
+        "portalEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustStoreResponseTypeDef = TypedDict(
+    "CreateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserSettingsResponseTypeDef = TypedDict(
+    "CreateUserSettingsResponseTypeDef",
+    {
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    {
+        "portalArn": str,
+        "serviceProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustStoreResponseTypeDef = TypedDict(
+    "UpdateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "trustStoreArn": str,
+    },
+)
+_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "certificatesToAdd": Sequence[BlobTypeDef],
+        "certificatesToDelete": Sequence[str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateTrustStoreRequestRequestTypeDef(
+    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
+):
+    pass
+
+
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBrowserSettingsResponseTypeDef = TypedDict(
     "GetBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBrowserSettingsResponseTypeDef = TypedDict(
     "UpdateBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoreCertificatesResponseTypeDef = TypedDict(
     "ListTrustStoreCertificatesResponseTypeDef",
     {
         "certificateList": List[CertificateSummaryTypeDef],
         "nextToken": str,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreCertificateResponseTypeDef = TypedDict(
     "GetTrustStoreCertificateResponseTypeDef",
     {
         "certificate": CertificateTypeDef,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrowserSettingsRequestRequestTypeDef",
     {
         "browserPolicy": str,
@@ -1232,15 +1234,15 @@
     },
     total=False,
 )
 
 _RequiredCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustStoreRequestRequestTypeDef",
     {
-        "certificateList": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        "certificateList": Sequence[BlobTypeDef],
     },
 )
 _OptionalCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrustStoreRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
@@ -1307,15 +1309,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1412,169 +1414,169 @@
     pass
 
 
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkSettingsResponseTypeDef = TypedDict(
     "GetNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkSettingsResponseTypeDef = TypedDict(
     "UpdateNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPortalResponseTypeDef = TypedDict(
     "GetPortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreResponseTypeDef = TypedDict(
     "GetTrustStoreResponseTypeDef",
     {
         "trustStore": TrustStoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "GetUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsResponseTypeDef = TypedDict(
     "UpdateUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "identityProviders": List[IdentityProviderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpAccessSettingsResponseTypeDef = TypedDict(
     "ListIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "ListUserAccessLoggingSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userAccessLoggingSettings": List[UserAccessLoggingSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserSettingsResponseTypeDef = TypedDict(
     "ListUserSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userSettings": List[UserSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIpAccessSettingsResponseTypeDef = TypedDict(
     "GetIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIpAccessSettingsResponseTypeDef = TypedDict(
     "UpdateIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web/type_defs.pyi` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef
 
-    data: AssociateBrowserSettingsRequestRequestTypeDef = {...}
+    data: AssociateBrowserSettingsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -31,40 +31,28 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
-    "AssociateBrowserSettingsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
-    "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
-    "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
-    "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
-    "AssociateUserSettingsResponseTypeDef",
+    "BlobTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
-    "CreateBrowserSettingsResponseTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
     "IpRuleTypeDef",
-    "CreateIpAccessSettingsResponseTypeDef",
-    "CreateNetworkSettingsResponseTypeDef",
-    "CreatePortalResponseTypeDef",
-    "CreateTrustStoreResponseTypeDef",
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    "CreateUserSettingsResponseTypeDef",
     "DeleteBrowserSettingsRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
     "DeleteIpAccessSettingsRequestRequestTypeDef",
     "DeleteNetworkSettingsRequestRequestTypeDef",
     "DeletePortalRequestRequestTypeDef",
     "DeleteTrustStoreRequestRequestTypeDef",
     "DeleteUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -80,15 +68,14 @@
     "IdentityProviderTypeDef",
     "GetIpAccessSettingsRequestRequestTypeDef",
     "GetNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsTypeDef",
     "GetPortalRequestRequestTypeDef",
     "PortalTypeDef",
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
-    "GetPortalServiceProviderMetadataResponseTypeDef",
     "GetTrustStoreCertificateRequestRequestTypeDef",
     "GetTrustStoreRequestRequestTypeDef",
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
@@ -105,24 +92,38 @@
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
-    "UpdateTrustStoreRequestRequestTypeDef",
-    "UpdateTrustStoreResponseTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
+    "AssociateBrowserSettingsResponseTypeDef",
+    "AssociateIpAccessSettingsResponseTypeDef",
+    "AssociateNetworkSettingsResponseTypeDef",
+    "AssociateTrustStoreResponseTypeDef",
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    "AssociateUserSettingsResponseTypeDef",
+    "CreateBrowserSettingsResponseTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "CreateIpAccessSettingsResponseTypeDef",
+    "CreateNetworkSettingsResponseTypeDef",
+    "CreatePortalResponseTypeDef",
+    "CreateTrustStoreResponseTypeDef",
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    "CreateUserSettingsResponseTypeDef",
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    "UpdateTrustStoreResponseTypeDef",
+    "UpdateTrustStoreRequestRequestTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
@@ -161,108 +162,66 @@
     "AssociateBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateBrowserSettingsResponseTypeDef = TypedDict(
-    "AssociateBrowserSettingsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "browserSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateIpAccessSettingsResponseTypeDef = TypedDict(
-    "AssociateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "AssociateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateNetworkSettingsResponseTypeDef = TypedDict(
-    "AssociateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateTrustStoreRequestRequestTypeDef = TypedDict(
     "AssociateTrustStoreRequestRequestTypeDef",
     {
         "portalArn": str,
         "trustStoreArn": str,
     },
 )
 
-AssociateTrustStoreResponseTypeDef = TypedDict(
-    "AssociateTrustStoreResponseTypeDef",
-    {
-        "portalArn": str,
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userAccessLoggingSettingsArn": str,
     },
 )
 
-AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
-AssociateUserSettingsResponseTypeDef = TypedDict(
-    "AssociateUserSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -314,22 +273,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateBrowserSettingsResponseTypeDef = TypedDict(
-    "CreateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
         "portalArn": str,
@@ -345,22 +296,14 @@
 
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
-    {
-        "identityProviderArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIpRuleTypeDef = TypedDict(
     "_RequiredIpRuleTypeDef",
     {
         "ipRange": str,
     },
 )
 _OptionalIpRuleTypeDef = TypedDict(
@@ -370,63 +313,14 @@
     },
     total=False,
 )
 
 class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
     pass
 
-CreateIpAccessSettingsResponseTypeDef = TypedDict(
-    "CreateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkSettingsResponseTypeDef = TypedDict(
-    "CreateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePortalResponseTypeDef = TypedDict(
-    "CreatePortalResponseTypeDef",
-    {
-        "portalArn": str,
-        "portalEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTrustStoreResponseTypeDef = TypedDict(
-    "CreateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserSettingsResponseTypeDef = TypedDict(
-    "CreateUserSettingsResponseTypeDef",
-    {
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
@@ -620,23 +514,14 @@
 GetPortalServiceProviderMetadataRequestRequestTypeDef = TypedDict(
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
-GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    {
-        "portalArn": str,
-        "serviceProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrustStoreCertificateRequestRequestTypeDef = TypedDict(
     "GetTrustStoreCertificateRequestRequestTypeDef",
     {
         "thumbprint": str,
         "trustStoreArn": str,
     },
 )
@@ -906,25 +791,14 @@
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
         "userSettingsArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1012,43 +886,14 @@
 )
 
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "trustStoreArn": str,
-    },
-)
-_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-        "certificatesToDelete": Sequence[str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class UpdateTrustStoreRequestRequestTypeDef(
-    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
-):
-    pass
-
-UpdateTrustStoreResponseTypeDef = TypedDict(
-    "UpdateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1089,55 +934,212 @@
 
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
+AssociateBrowserSettingsResponseTypeDef = TypedDict(
+    "AssociateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateIpAccessSettingsResponseTypeDef = TypedDict(
+    "AssociateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateNetworkSettingsResponseTypeDef = TypedDict(
+    "AssociateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateTrustStoreResponseTypeDef = TypedDict(
+    "AssociateTrustStoreResponseTypeDef",
+    {
+        "portalArn": str,
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserSettingsResponseTypeDef = TypedDict(
+    "AssociateUserSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBrowserSettingsResponseTypeDef = TypedDict(
+    "CreateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
+    {
+        "identityProviderArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIpAccessSettingsResponseTypeDef = TypedDict(
+    "CreateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkSettingsResponseTypeDef = TypedDict(
+    "CreateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortalResponseTypeDef = TypedDict(
+    "CreatePortalResponseTypeDef",
+    {
+        "portalArn": str,
+        "portalEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustStoreResponseTypeDef = TypedDict(
+    "CreateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserSettingsResponseTypeDef = TypedDict(
+    "CreateUserSettingsResponseTypeDef",
+    {
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    {
+        "portalArn": str,
+        "serviceProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustStoreResponseTypeDef = TypedDict(
+    "UpdateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "trustStoreArn": str,
+    },
+)
+_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "certificatesToAdd": Sequence[BlobTypeDef],
+        "certificatesToDelete": Sequence[str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateTrustStoreRequestRequestTypeDef(
+    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
+):
+    pass
+
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBrowserSettingsResponseTypeDef = TypedDict(
     "GetBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBrowserSettingsResponseTypeDef = TypedDict(
     "UpdateBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoreCertificatesResponseTypeDef = TypedDict(
     "ListTrustStoreCertificatesResponseTypeDef",
     {
         "certificateList": List[CertificateSummaryTypeDef],
         "nextToken": str,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreCertificateResponseTypeDef = TypedDict(
     "GetTrustStoreCertificateResponseTypeDef",
     {
         "certificate": CertificateTypeDef,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrowserSettingsRequestRequestTypeDef",
     {
         "browserPolicy": str,
@@ -1195,15 +1197,15 @@
     },
     total=False,
 )
 
 _RequiredCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustStoreRequestRequestTypeDef",
     {
-        "certificateList": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        "certificateList": Sequence[BlobTypeDef],
     },
 )
 _OptionalCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrustStoreRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
@@ -1264,15 +1266,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1361,169 +1363,169 @@
 ):
     pass
 
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkSettingsResponseTypeDef = TypedDict(
     "GetNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkSettingsResponseTypeDef = TypedDict(
     "UpdateNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPortalResponseTypeDef = TypedDict(
     "GetPortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreResponseTypeDef = TypedDict(
     "GetTrustStoreResponseTypeDef",
     {
         "trustStore": TrustStoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "GetUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsResponseTypeDef = TypedDict(
     "UpdateUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "identityProviders": List[IdentityProviderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpAccessSettingsResponseTypeDef = TypedDict(
     "ListIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "ListUserAccessLoggingSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userAccessLoggingSettings": List[UserAccessLoggingSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserSettingsResponseTypeDef = TypedDict(
     "ListUserSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userSettings": List[UserSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIpAccessSettingsResponseTypeDef = TypedDict(
     "GetIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIpAccessSettingsResponseTypeDef = TypedDict(
     "UpdateIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/PKG-INFO` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces-web
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore workspaces-web type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore workspaces-web type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-workspaces-web"></a>
 
 # types-aiobotocore-workspaces-web
 
 [![PyPI - types-aiobotocore-workspaces-web](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workspaces-web?color=blue)](https://pypistats.org/packages/types-aiobotocore-workspaces-web)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-web)](https://pepy.tech/project/types-aiobotocore-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkSpacesWeb 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [types-aiobotocore-workspaces-web docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/).
 
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
@@ -286,50 +285,38 @@
 )
 
 
 def check_value(value: AuthenticationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_workspaces_web.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
-    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
-    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
-    AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    CreateIdentityProviderResponseTypeDef,
     IpRuleTypeDef,
-    CreateIpAccessSettingsResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
@@ -345,15 +332,14 @@
     IdentityProviderTypeDef,
     GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
@@ -370,24 +356,38 @@
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
-    UpdateTrustStoreRequestRequestTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
+    AssociateTrustStoreResponseTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
+    AssociateUserSettingsResponseTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
+    UpdateTrustStoreResponseTypeDef,
+    UpdateTrustStoreRequestRequestTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
@@ -419,15 +419,15 @@
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
+def get_value() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*


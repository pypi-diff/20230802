# Comparing `tmp/types-aiobotocore-rolesanywhere-2.5.2.tar.gz` & `tmp/types-aiobotocore-rolesanywhere-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rolesanywhere-2.5.2.tar", last modified: Sat Jul  8 01:44:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-rolesanywhere-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
```

## Comparing `types-aiobotocore-rolesanywhere-2.5.2.tar` & `types-aiobotocore-rolesanywhere-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:12.858789 types-aiobotocore-rolesanywhere-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-07-08 01:44:12.858789 types-aiobotocore-rolesanywhere-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:12.858789 types-aiobotocore-rolesanywhere-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:12.854789 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:24.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:12.858789 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-07-08 01:44:12.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:44:12.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:12.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:12.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:12.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:44:12.000000 types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.181477 types-aiobotocore-rolesanywhere-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-02 14:52:54.173477 types-aiobotocore-rolesanywhere-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.181477 types-aiobotocore-rolesanywhere-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.173477 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-08-02 14:48:00.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-08-02 14:48:00.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-08-02 14:48:00.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.173477 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-02 14:52:53.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:53.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/LICENSE` & `types-aiobotocore-rolesanywhere-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore rolesanywhere type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rolesanywhere"></a>
 
 # types-aiobotocore-rolesanywhere
 
 [![PyPI - types-aiobotocore-rolesanywhere](https://img.shields.io/pypi/v/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rolesanywhere?color=blue)](https://pypistats.org/packages/types-aiobotocore-rolesanywhere)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IAMRolesAnywhere 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
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
@@ -321,73 +320,74 @@
 )
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_rolesanywhere.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_rolesanywhere.type_defs import (
+    BlobTypeDef,
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
+    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
+    UpdateCrlRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/README.md` & `types-aiobotocore-rolesanywhere-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-rolesanywhere"></a>
 
 # types-aiobotocore-rolesanywhere
 
 [![PyPI - types-aiobotocore-rolesanywhere](https://img.shields.io/pypi/v/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rolesanywhere?color=blue)](https://pypistats.org/packages/types-aiobotocore-rolesanywhere)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IAMRolesAnywhere 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
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
@@ -288,73 +288,74 @@
 )
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_rolesanywhere.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_rolesanywhere.type_defs import (
+    BlobTypeDef,
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
+    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
+    UpdateCrlRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/setup.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rolesanywhere",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with"
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
-    keywords="aiobotocore rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore rolesanywhere type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rolesanywhere": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/"
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/__init__.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/__init__.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/__main__.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/client.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
     session = get_session()
     async with session.create_client("rolesanywhere") as client:
         client: IAMRolesAnywhereClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .paginator import (
     ListCrlsPaginator,
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
     NotificationSettingKeyTypeDef,
@@ -258,15 +258,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_trust_anchor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#get_trust_anchor)
         """
 
     async def import_crl(
         self,
         *,
-        crlData: Union[str, bytes, IO[Any], StreamingBody],
+        crlData: BlobTypeDef,
         name: str,
         trustAnchorArn: str,
         enabled: bool = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Imports the certificate revocation list (CRL).
@@ -363,19 +363,15 @@
         Removes tags from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#untag_resource)
         """
 
     async def update_crl(
-        self,
-        *,
-        crlId: str,
-        crlData: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        name: str = ...
+        self, *, crlId: str, crlData: BlobTypeDef = ..., name: str = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Updates the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_crl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#update_crl)
         """
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/client.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
     session = get_session()
     async with session.create_client("rolesanywhere") as client:
         client: IAMRolesAnywhereClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .paginator import (
     ListCrlsPaginator,
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
     NotificationSettingKeyTypeDef,
@@ -235,15 +235,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_trust_anchor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#get_trust_anchor)
         """
     async def import_crl(
         self,
         *,
-        crlData: Union[str, bytes, IO[Any], StreamingBody],
+        crlData: BlobTypeDef,
         name: str,
         trustAnchorArn: str,
         enabled: bool = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Imports the certificate revocation list (CRL).
@@ -330,19 +330,15 @@
         """
         Removes tags from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#untag_resource)
         """
     async def update_crl(
-        self,
-        *,
-        crlId: str,
-        crlData: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        name: str = ...
+        self, *, crlId: str, crlData: BlobTypeDef = ..., name: str = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Updates the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_crl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#update_crl)
         """
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/literals.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/literals.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/paginator.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -42,76 +42,70 @@
 __all__ = (
     "ListCrlsPaginator",
     "ListProfilesPaginator",
     "ListSubjectsPaginator",
     "ListTrustAnchorsPaginator",
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
 class ListCrlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listcrlspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCrlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listcrlspaginator)
         """
 
-
 class ListProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listprofilespaginator)
         """
 
-
 class ListSubjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listsubjectspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSubjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listsubjectspaginator)
         """
 
-
 class ListTrustAnchorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listtrustanchorspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrustAnchorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listtrustanchorspaginator)
         """
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/paginator.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,70 +42,76 @@
 __all__ = (
     "ListCrlsPaginator",
     "ListProfilesPaginator",
     "ListSubjectsPaginator",
     "ListTrustAnchorsPaginator",
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
 class ListCrlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listcrlspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCrlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listcrlspaginator)
         """
 
+
 class ListProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listprofilespaginator)
         """
 
+
 class ListSubjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listsubjectspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSubjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listsubjectspaginator)
         """
 
+
 class ListTrustAnchorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listtrustanchorspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrustAnchorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/paginators/#listtrustanchorspaginator)
         """
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/type_defs.py` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for rolesanywhere service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_rolesanywhere.type_defs import TagTypeDef
+    from types_aiobotocore_rolesanywhere.type_defs import BlobTypeDef
 
-    data: TagTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -26,62 +26,64 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
-    "ListRequestListCrlsPaginateTypeDef",
-    "ListRequestListProfilesPaginateTypeDef",
-    "ListRequestListSubjectsPaginateTypeDef",
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
+    "UpdateCrlRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
+    "ListRequestListCrlsPaginateTypeDef",
+    "ListRequestListProfilesPaginateTypeDef",
+    "ListRequestListSubjectsPaginateTypeDef",
+    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -133,14 +135,25 @@
         "name": str,
         "trustAnchorArn": str,
         "updatedAt": datetime,
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
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": bool,
         "properties": Dict[str, str],
         "seenAt": datetime,
     },
@@ -162,46 +175,20 @@
         "roleArns": List[str],
         "sessionPolicy": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListRequestListCrlsPaginateTypeDef = TypedDict(
-    "ListRequestListCrlsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListRequestListProfilesPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListSubjectsPaginateTypeDef = TypedDict(
-    "ListRequestListSubjectsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRequestRequestTypeDef = TypedDict(
     "ListRequestRequestTypeDef",
     {
@@ -273,35 +260,14 @@
 
 class NotificationSettingKeyTypeDef(
     _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
 ):
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
-
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -339,57 +305,57 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCrlRequestRequestTypeDef",
+_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProfileRequestRequestTypeDef",
     {
-        "crlId": str,
+        "profileId": str,
     },
 )
-_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCrlRequestRequestTypeDef",
+_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProfileRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "durationSeconds": int,
+        "managedPolicyArns": Sequence[str],
         "name": str,
+        "roleArns": Sequence[str],
+        "sessionPolicy": str,
     },
     total=False,
 )
 
 
-class UpdateCrlRequestRequestTypeDef(
-    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
+class UpdateProfileRequestRequestTypeDef(
+    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProfileRequestRequestTypeDef",
+_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCrlRequestRequestTypeDef",
     {
-        "profileId": str,
+        "crlId": str,
     },
 )
-_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProfileRequestRequestTypeDef",
+_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCrlRequestRequestTypeDef",
     {
-        "durationSeconds": int,
-        "managedPolicyArns": Sequence[str],
+        "crlData": BlobTypeDef,
         "name": str,
-        "roleArns": Sequence[str],
-        "sessionPolicy": str,
     },
     total=False,
 )
 
 
-class UpdateProfileRequestRequestTypeDef(
-    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
+class UpdateCrlRequestRequestTypeDef(
+    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
@@ -416,15 +382,15 @@
 ):
     pass
 
 
 _RequiredImportCrlRequestRequestTypeDef = TypedDict(
     "_RequiredImportCrlRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "crlData": BlobTypeDef,
         "name": str,
         "trustAnchorArn": str,
     },
 )
 _OptionalImportCrlRequestRequestTypeDef = TypedDict(
     "_OptionalImportCrlRequestRequestTypeDef",
     {
@@ -437,22 +403,14 @@
 
 class ImportCrlRequestRequestTypeDef(
     _RequiredImportCrlRequestRequestTypeDef, _OptionalImportCrlRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -465,24 +423,32 @@
     },
 )
 
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCrlsResponseTypeDef = TypedDict(
     "ListCrlsResponseTypeDef",
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
@@ -499,32 +465,68 @@
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "nextToken": str,
         "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProfileDetailResponseTypeDef = TypedDict(
     "ProfileDetailResponseTypeDef",
     {
         "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRequestListCrlsPaginateTypeDef = TypedDict(
+    "ListRequestListCrlsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListRequestListProfilesPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListSubjectsPaginateTypeDef = TypedDict(
+    "ListRequestListSubjectsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
+    "ListRequestListTrustAnchorsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSubjectsResponseTypeDef = TypedDict(
     "ListSubjectsResponseTypeDef",
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
@@ -541,15 +543,15 @@
     total=False,
 )
 
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
@@ -611,34 +613,34 @@
 
 
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutNotificationSettingsResponseTypeDef = TypedDict(
     "PutNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsResponseTypeDef = TypedDict(
     "ResetNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere/type_defs.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for rolesanywhere service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_rolesanywhere.type_defs import TagTypeDef
+    from types_aiobotocore_rolesanywhere.type_defs import BlobTypeDef
 
-    data: TagTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -25,62 +25,64 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
-    "ListRequestListCrlsPaginateTypeDef",
-    "ListRequestListProfilesPaginateTypeDef",
-    "ListRequestListSubjectsPaginateTypeDef",
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
+    "UpdateCrlRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
+    "ListRequestListCrlsPaginateTypeDef",
+    "ListRequestListProfilesPaginateTypeDef",
+    "ListRequestListSubjectsPaginateTypeDef",
+    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -130,14 +132,25 @@
         "name": str,
         "trustAnchorArn": str,
         "updatedAt": datetime,
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
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": bool,
         "properties": Dict[str, str],
         "seenAt": datetime,
     },
@@ -159,46 +172,20 @@
         "roleArns": List[str],
         "sessionPolicy": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListRequestListCrlsPaginateTypeDef = TypedDict(
-    "ListRequestListCrlsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListRequestListProfilesPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListSubjectsPaginateTypeDef = TypedDict(
-    "ListRequestListSubjectsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRequestRequestTypeDef = TypedDict(
     "ListRequestRequestTypeDef",
     {
@@ -266,35 +253,14 @@
 )
 
 class NotificationSettingKeyTypeDef(
     _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
 ):
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
-
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -332,54 +298,54 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCrlRequestRequestTypeDef",
+_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProfileRequestRequestTypeDef",
     {
-        "crlId": str,
+        "profileId": str,
     },
 )
-_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCrlRequestRequestTypeDef",
+_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProfileRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "durationSeconds": int,
+        "managedPolicyArns": Sequence[str],
         "name": str,
+        "roleArns": Sequence[str],
+        "sessionPolicy": str,
     },
     total=False,
 )
 
-class UpdateCrlRequestRequestTypeDef(
-    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
+class UpdateProfileRequestRequestTypeDef(
+    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProfileRequestRequestTypeDef",
+_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCrlRequestRequestTypeDef",
     {
-        "profileId": str,
+        "crlId": str,
     },
 )
-_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProfileRequestRequestTypeDef",
+_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCrlRequestRequestTypeDef",
     {
-        "durationSeconds": int,
-        "managedPolicyArns": Sequence[str],
+        "crlData": BlobTypeDef,
         "name": str,
-        "roleArns": Sequence[str],
-        "sessionPolicy": str,
     },
     total=False,
 )
 
-class UpdateProfileRequestRequestTypeDef(
-    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
+class UpdateCrlRequestRequestTypeDef(
+    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
 ):
     pass
 
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
         "name": str,
@@ -403,15 +369,15 @@
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
 ):
     pass
 
 _RequiredImportCrlRequestRequestTypeDef = TypedDict(
     "_RequiredImportCrlRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "crlData": BlobTypeDef,
         "name": str,
         "trustAnchorArn": str,
     },
 )
 _OptionalImportCrlRequestRequestTypeDef = TypedDict(
     "_OptionalImportCrlRequestRequestTypeDef",
     {
@@ -422,22 +388,14 @@
 )
 
 class ImportCrlRequestRequestTypeDef(
     _RequiredImportCrlRequestRequestTypeDef, _OptionalImportCrlRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -450,24 +408,32 @@
     },
 )
 
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCrlsResponseTypeDef = TypedDict(
     "ListCrlsResponseTypeDef",
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
@@ -484,32 +450,68 @@
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "nextToken": str,
         "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProfileDetailResponseTypeDef = TypedDict(
     "ProfileDetailResponseTypeDef",
     {
         "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRequestListCrlsPaginateTypeDef = TypedDict(
+    "ListRequestListCrlsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListRequestListProfilesPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListSubjectsPaginateTypeDef = TypedDict(
+    "ListRequestListSubjectsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
+    "ListRequestListTrustAnchorsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSubjectsResponseTypeDef = TypedDict(
     "ListSubjectsResponseTypeDef",
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
@@ -526,15 +528,15 @@
     total=False,
 )
 
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
@@ -592,34 +594,34 @@
     pass
 
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutNotificationSettingsResponseTypeDef = TypedDict(
     "PutNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsResponseTypeDef = TypedDict(
     "ResetNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore rolesanywhere type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rolesanywhere"></a>
 
 # types-aiobotocore-rolesanywhere
 
 [![PyPI - types-aiobotocore-rolesanywhere](https://img.shields.io/pypi/v/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rolesanywhere?color=blue)](https://pypistats.org/packages/types-aiobotocore-rolesanywhere)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IAMRolesAnywhere 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
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
@@ -321,73 +320,74 @@
 )
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_rolesanywhere.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_rolesanywhere.type_defs import (
+    BlobTypeDef,
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
+    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
+    UpdateCrlRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt` & `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*


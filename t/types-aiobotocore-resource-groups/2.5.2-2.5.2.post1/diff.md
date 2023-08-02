# Comparing `tmp/types-aiobotocore-resource-groups-2.5.2.tar.gz` & `tmp/types-aiobotocore-resource-groups-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resource-groups-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-resource-groups-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-resource-groups-2.5.2.tar` & `types-aiobotocore-resource-groups-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.930772 types-aiobotocore-resource-groups-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-07-08 01:44:11.930772 types-aiobotocore-resource-groups-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.930772 types-aiobotocore-resource-groups-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.926772 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16961 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:17.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.930772 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-07-08 01:44:11.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:44:11.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:44:11.000000 types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.905481 types-aiobotocore-resource-groups-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-08-02 14:52:52.893481 types-aiobotocore-resource-groups-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.905481 types-aiobotocore-resource-groups-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.889481 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/LICENSE` & `types-aiobotocore-resource-groups-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2/PKG-INFO` & `types-aiobotocore-resource-groups-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-groups
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resource-groups type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resource-groups type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resource-groups?color=blue)](https://pypistats.org/packages/types-aiobotocore-resource-groups)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-groups)](https://pepy.tech/project/types-aiobotocore-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceGroups 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
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
@@ -323,82 +322,85 @@
 )
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resource_groups.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
-    GetTagsOutputTypeDef,
+    GroupConfigurationParameterOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
+    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
-    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
-    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
     GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
     DeleteGroupOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
+    GetTagsOutputTypeDef,
+    TagOutputTypeDef,
+    UntagOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
     GroupConfigurationTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
+    CreateGroupInputRequestTypeDef,
+    PutGroupConfigurationInputRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/README.md` & `types-aiobotocore-resource-groups-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resource-groups?color=blue)](https://pypistats.org/packages/types-aiobotocore-resource-groups)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-groups)](https://pepy.tech/project/types-aiobotocore-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceGroups 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
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
@@ -290,82 +290,85 @@
 )
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resource_groups.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
-    GetTagsOutputTypeDef,
+    GroupConfigurationParameterOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
+    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
-    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
-    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
     GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
     DeleteGroupOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
+    GetTagsOutputTypeDef,
+    TagOutputTypeDef,
+    UntagOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
     GroupConfigurationTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
+    CreateGroupInputRequestTypeDef,
+    PutGroupConfigurationInputRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/setup.py` & `types-aiobotocore-resource-groups-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resource-groups",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with"
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
-    keywords="aiobotocore resource-groups type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore resource-groups type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resource_groups": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/"
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/__init__.py` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/__init__.pyi` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/__main__.py` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResourceGroups 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ResourceGroups 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
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

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/client.py` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
-    GroupConfigurationItemTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
@@ -110,15 +110,15 @@
     async def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#create_group)
         """
@@ -231,15 +231,15 @@
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#list_groups)
         """
 
     async def put_group_configuration(
-        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/client.pyi` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
-    GroupConfigurationItemTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
@@ -103,15 +103,15 @@
     async def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#create_group)
         """
@@ -213,15 +213,15 @@
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#list_groups)
         """
     async def put_group_configuration(
-        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/literals.py` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/literals.pyi` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/paginator.py` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 
@@ -78,31 +78,28 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
         """
 
 
 class SearchResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#searchresourcespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ResourceQuery: ResourceQueryTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceQuery: ResourceQueryTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/paginator.pyi` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
@@ -74,30 +74,27 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
         """
 
 class SearchResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#searchresourcespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ResourceQuery: ResourceQueryTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceQuery: ResourceQueryTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/type_defs.py` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GroupConfigurationStatusType,
     GroupFilterNameType,
     GroupLifecycleEventsDesiredStatusType,
     GroupLifecycleEventsStatusType,
     QueryErrorCodeType,
@@ -33,66 +33,69 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
-    "GetTagsOutputTypeDef",
+    "GroupConfigurationParameterOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagInputRequestTypeDef",
-    "TagOutputTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
-    "UntagOutputTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
-    "GetAccountSettingsOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
     "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
-    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
     "DeleteGroupOutputTypeDef",
+    "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
+    "GetTagsOutputTypeDef",
+    "TagOutputTypeDef",
+    "UntagOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
+    "GroupConfigurationItemOutputTypeDef",
     "GroupConfigurationItemTypeDef",
-    "ListGroupsInputListGroupsPaginateTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
-    "CreateGroupInputRequestTypeDef",
     "GroupConfigurationTypeDef",
-    "PutGroupConfigurationInputRequestTypeDef",
+    "GroupConfigurationItemUnionTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
+    "CreateGroupInputRequestTypeDef",
+    "PutGroupConfigurationInputRequestTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
         "GroupLifecycleEventsStatus": GroupLifecycleEventsStatusType,
@@ -125,14 +128,25 @@
 )
 
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
 
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
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
@@ -177,22 +191,35 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetTagsOutputTypeDef = TypedDict(
-    "GetTagsOutputTypeDef",
+_RequiredGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationParameterOutputTypeDef",
     {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
+_OptionalGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationParameterOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
+
+class GroupConfigurationParameterOutputTypeDef(
+    _RequiredGroupConfigurationParameterOutputTypeDef,
+    _OptionalGroupConfigurationParameterOutputTypeDef,
+):
+    pass
+
 
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
@@ -240,14 +267,24 @@
     "PendingResourceTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ResourceFilterTypeDef = TypedDict(
     "ResourceFilterTypeDef",
     {
         "Name": Literal["resource-type"],
         "Values": Sequence[str],
     },
 )
@@ -274,52 +311,22 @@
     {
         "ErrorCode": QueryErrorCodeType,
         "Message": str,
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
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 TagInputRequestTypeDef = TypedDict(
     "TagInputRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UngroupResourcesInputRequestTypeDef = TypedDict(
     "UngroupResourcesInputRequestTypeDef",
     {
         "Group": str,
         "ResourceArns": Sequence[str],
     },
 )
@@ -328,23 +335,14 @@
     "UntagInputRequestTypeDef",
     {
         "Arn": str,
         "Keys": Sequence[str],
     },
 )
 
-UntagOutputTypeDef = TypedDict(
-    "UntagOutputTypeDef",
-    {
-        "Arn": str,
-        "Keys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
     },
     total=False,
 )
@@ -355,30 +353,14 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupQueryTypeDef = TypedDict(
     "GroupQueryTypeDef",
     {
         "GroupName": str,
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
@@ -401,36 +383,14 @@
 
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
 
-_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchResourcesInputSearchResourcesPaginateTypeDef(
-    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
-    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -449,34 +409,98 @@
     pass
 
 
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupOutputTypeDef = TypedDict(
     "GetGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsOutputTypeDef = TypedDict(
+    "GetTagsOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagOutputTypeDef = TypedDict(
+    "UntagOutputTypeDef",
+    {
+        "Arn": str,
+        "Keys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupOutputTypeDef = TypedDict(
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationItemOutputTypeDef",
+    {
+        "Type": str,
+    },
+)
+_OptionalGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationItemOutputTypeDef",
+    {
+        "Parameters": List[GroupConfigurationParameterOutputTypeDef],
     },
+    total=False,
 )
 
+
+class GroupConfigurationItemOutputTypeDef(
+    _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
+):
+    pass
+
+
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
@@ -490,23 +514,14 @@
 
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
 
-ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[GroupFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -515,45 +530,76 @@
 
 ListGroupsOutputTypeDef = TypedDict(
     "ListGroupsOutputTypeDef",
     {
         "GroupIdentifiers": List[GroupIdentifierTypeDef],
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupResourcesOutputTypeDef = TypedDict(
     "GroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UngroupResourcesOutputTypeDef = TypedDict(
     "UngroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[GroupFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchResourcesInputSearchResourcesPaginateTypeDef(
+    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
+    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
+):
+    pass
+
+
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListGroupResourcesInputRequestTypeDef = TypedDict(
     "ListGroupResourcesInputRequestTypeDef",
     {
@@ -577,100 +623,103 @@
 
 SearchResourcesOutputTypeDef = TypedDict(
     "SearchResourcesOutputTypeDef",
     {
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupQueryOutputTypeDef = TypedDict(
     "GetGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupQueryOutputTypeDef = TypedDict(
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGroupInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGroupInputRequestTypeDef",
-    {
-        "Description": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-        "Tags": Mapping[str, str],
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateGroupInputRequestTypeDef(
-    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
-):
-    pass
-
-
 GroupConfigurationTypeDef = TypedDict(
     "GroupConfigurationTypeDef",
     {
-        "Configuration": List[GroupConfigurationItemTypeDef],
-        "ProposedConfiguration": List[GroupConfigurationItemTypeDef],
+        "Configuration": List[GroupConfigurationItemOutputTypeDef],
+        "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
         "Status": GroupConfigurationStatusType,
         "FailureReason": str,
     },
     total=False,
 )
 
-PutGroupConfigurationInputRequestTypeDef = TypedDict(
-    "PutGroupConfigurationInputRequestTypeDef",
-    {
-        "Group": str,
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
-    },
-    total=False,
-)
-
+GroupConfigurationItemUnionTypeDef = Union[
+    GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef
+]
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGroupInputRequestTypeDef",
+    {
+        "Name": str,
     },
 )
+_OptionalCreateGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGroupInputRequestTypeDef",
+    {
+        "Description": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+        "Tags": Mapping[str, str],
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateGroupInputRequestTypeDef(
+    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
+):
+    pass
+
+
+PutGroupConfigurationInputRequestTypeDef = TypedDict(
+    "PutGroupConfigurationInputRequestTypeDef",
+    {
+        "Group": str,
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
+    },
+    total=False,
+)
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups/type_defs.pyi` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GroupConfigurationStatusType,
     GroupFilterNameType,
     GroupLifecycleEventsDesiredStatusType,
     GroupLifecycleEventsStatusType,
     QueryErrorCodeType,
@@ -32,66 +32,69 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
-    "GetTagsOutputTypeDef",
+    "GroupConfigurationParameterOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagInputRequestTypeDef",
-    "TagOutputTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
-    "UntagOutputTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
-    "GetAccountSettingsOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
     "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
-    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
     "DeleteGroupOutputTypeDef",
+    "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
+    "GetTagsOutputTypeDef",
+    "TagOutputTypeDef",
+    "UntagOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
+    "GroupConfigurationItemOutputTypeDef",
     "GroupConfigurationItemTypeDef",
-    "ListGroupsInputListGroupsPaginateTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
-    "CreateGroupInputRequestTypeDef",
     "GroupConfigurationTypeDef",
-    "PutGroupConfigurationInputRequestTypeDef",
+    "GroupConfigurationItemUnionTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
+    "CreateGroupInputRequestTypeDef",
+    "PutGroupConfigurationInputRequestTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
         "GroupLifecycleEventsStatus": GroupLifecycleEventsStatusType,
@@ -122,14 +125,25 @@
     },
     total=False,
 )
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
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
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
@@ -174,22 +188,33 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetTagsOutputTypeDef = TypedDict(
-    "GetTagsOutputTypeDef",
+_RequiredGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationParameterOutputTypeDef",
     {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
+_OptionalGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationParameterOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
+class GroupConfigurationParameterOutputTypeDef(
+    _RequiredGroupConfigurationParameterOutputTypeDef,
+    _OptionalGroupConfigurationParameterOutputTypeDef,
+):
+    pass
 
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
@@ -235,14 +260,24 @@
     "PendingResourceTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ResourceFilterTypeDef = TypedDict(
     "ResourceFilterTypeDef",
     {
         "Name": Literal["resource-type"],
         "Values": Sequence[str],
     },
 )
@@ -269,52 +304,22 @@
     {
         "ErrorCode": QueryErrorCodeType,
         "Message": str,
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
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 TagInputRequestTypeDef = TypedDict(
     "TagInputRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UngroupResourcesInputRequestTypeDef = TypedDict(
     "UngroupResourcesInputRequestTypeDef",
     {
         "Group": str,
         "ResourceArns": Sequence[str],
     },
 )
@@ -323,23 +328,14 @@
     "UntagInputRequestTypeDef",
     {
         "Arn": str,
         "Keys": Sequence[str],
     },
 )
 
-UntagOutputTypeDef = TypedDict(
-    "UntagOutputTypeDef",
-    {
-        "Arn": str,
-        "Keys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
     },
     total=False,
 )
@@ -350,30 +346,14 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupQueryTypeDef = TypedDict(
     "GroupQueryTypeDef",
     {
         "GroupName": str,
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
@@ -394,34 +374,14 @@
 )
 
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
-_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchResourcesInputSearchResourcesPaginateTypeDef(
-    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
-    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -438,34 +398,96 @@
 ):
     pass
 
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupOutputTypeDef = TypedDict(
     "GetGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsOutputTypeDef = TypedDict(
+    "GetTagsOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagOutputTypeDef = TypedDict(
+    "UntagOutputTypeDef",
+    {
+        "Arn": str,
+        "Keys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupOutputTypeDef = TypedDict(
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationItemOutputTypeDef",
+    {
+        "Type": str,
+    },
+)
+_OptionalGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationItemOutputTypeDef",
+    {
+        "Parameters": List[GroupConfigurationParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class GroupConfigurationItemOutputTypeDef(
+    _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
+):
+    pass
+
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
@@ -477,23 +499,14 @@
 )
 
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
-ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[GroupFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -502,45 +515,74 @@
 
 ListGroupsOutputTypeDef = TypedDict(
     "ListGroupsOutputTypeDef",
     {
         "GroupIdentifiers": List[GroupIdentifierTypeDef],
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupResourcesOutputTypeDef = TypedDict(
     "GroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UngroupResourcesOutputTypeDef = TypedDict(
     "UngroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[GroupFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class SearchResourcesInputSearchResourcesPaginateTypeDef(
+    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
+    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
+):
+    pass
+
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListGroupResourcesInputRequestTypeDef = TypedDict(
     "ListGroupResourcesInputRequestTypeDef",
     {
@@ -564,98 +606,101 @@
 
 SearchResourcesOutputTypeDef = TypedDict(
     "SearchResourcesOutputTypeDef",
     {
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupQueryOutputTypeDef = TypedDict(
     "GetGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupQueryOutputTypeDef = TypedDict(
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGroupInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGroupInputRequestTypeDef",
-    {
-        "Description": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-        "Tags": Mapping[str, str],
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateGroupInputRequestTypeDef(
-    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
-):
-    pass
-
 GroupConfigurationTypeDef = TypedDict(
     "GroupConfigurationTypeDef",
     {
-        "Configuration": List[GroupConfigurationItemTypeDef],
-        "ProposedConfiguration": List[GroupConfigurationItemTypeDef],
+        "Configuration": List[GroupConfigurationItemOutputTypeDef],
+        "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
         "Status": GroupConfigurationStatusType,
         "FailureReason": str,
     },
     total=False,
 )
 
-PutGroupConfigurationInputRequestTypeDef = TypedDict(
-    "PutGroupConfigurationInputRequestTypeDef",
-    {
-        "Group": str,
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
-    },
-    total=False,
-)
-
+GroupConfigurationItemUnionTypeDef = Union[
+    GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef
+]
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGroupInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGroupInputRequestTypeDef",
+    {
+        "Description": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+        "Tags": Mapping[str, str],
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateGroupInputRequestTypeDef(
+    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
+):
+    pass
+
+PutGroupConfigurationInputRequestTypeDef = TypedDict(
+    "PutGroupConfigurationInputRequestTypeDef",
+    {
+        "Group": str,
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
+    },
+    total=False,
+)
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/PKG-INFO` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-groups
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resource-groups type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resource-groups type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resource-groups?color=blue)](https://pypistats.org/packages/types-aiobotocore-resource-groups)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-groups)](https://pepy.tech/project/types-aiobotocore-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceGroups 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
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
@@ -323,82 +322,85 @@
 )
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resource_groups.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
-    GetTagsOutputTypeDef,
+    GroupConfigurationParameterOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
+    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
-    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
-    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
     GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
     DeleteGroupOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
+    GetTagsOutputTypeDef,
+    TagOutputTypeDef,
+    UntagOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
     GroupConfigurationTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
+    CreateGroupInputRequestTypeDef,
+    PutGroupConfigurationInputRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resource-groups-2.5.2/types_aiobotocore_resource_groups.egg-info/SOURCES.txt` & `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*


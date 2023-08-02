# Comparing `tmp/types-aiobotocore-codestar-notifications-2.5.2.tar.gz` & `tmp/types-aiobotocore-codestar-notifications-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-notifications-2.5.2.tar", last modified: Sat Jul  8 01:43:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-notifications-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
```

## Comparing `types-aiobotocore-codestar-notifications-2.5.2.tar` & `types-aiobotocore-codestar-notifications-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.837907 types-aiobotocore-codestar-notifications-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15502 2023-07-08 01:43:25.837907 types-aiobotocore-codestar-notifications-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:25.837907 types-aiobotocore-codestar-notifications-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.837907 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:43.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.837907 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15502 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.861618 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-02 14:35:17.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-08-02 14:35:17.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-02 14:35:17.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/LICENSE` & `types-aiobotocore-codestar-notifications-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.5.2.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar-notifications type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codestar-notifications type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar-notifications"></a>
 
 # types-aiobotocore-codestar-notifications
 
 [![PyPI - types-aiobotocore-codestar-notifications](https://img.shields.io/pypi/v/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar-notifications?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar-notifications)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStarNotifications 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
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
@@ -321,62 +320,63 @@
 )
 
 
 def check_value(value: DetailTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar_notifications.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_codestar_notifications.type_defs import (
     TargetTypeDef,
-    CreateNotificationRuleResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
-    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
+    CreateNotificationRuleResultTypeDef,
+    DeleteNotificationRuleResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    SubscribeResultTypeDef,
+    TagResourceResultTypeDef,
+    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListEventTypesRequestRequestTypeDef,
+    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TargetTypeDef:
+def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/README.md` & `types-aiobotocore-codestar-notifications-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codestar-notifications"></a>
 
 # types-aiobotocore-codestar-notifications
 
 [![PyPI - types-aiobotocore-codestar-notifications](https://img.shields.io/pypi/v/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar-notifications?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar-notifications)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStarNotifications 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
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
@@ -288,62 +288,63 @@
 )
 
 
 def check_value(value: DetailTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar_notifications.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_codestar_notifications.type_defs import (
     TargetTypeDef,
-    CreateNotificationRuleResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
-    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
+    CreateNotificationRuleResultTypeDef,
+    DeleteNotificationRuleResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    SubscribeResultTypeDef,
+    TagResourceResultTypeDef,
+    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListEventTypesRequestRequestTypeDef,
+    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TargetTypeDef:
+def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/setup.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-notifications",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codestar_notifications"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore codestar-notifications type-annotations boto3-stubs mypy typeshed autocomplete"
+        "aiobotocore codestar-notifications type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codestar_notifications": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/",
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/__init__.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/__init__.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/__main__.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeStarNotifications 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications\nOther"
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

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/client.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/client.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/literals.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/literals.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/paginator.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,70 +37,65 @@
     ListTargetsFilterTypeDef,
     ListTargetsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEventTypesPaginator", "ListNotificationRulesPaginator", "ListTargetsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEventTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
-
 class ListNotificationRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
-
 class ListTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/paginator.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,65 +37,70 @@
     ListTargetsFilterTypeDef,
     ListTargetsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEventTypesPaginator", "ListNotificationRulesPaginator", "ListTargetsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEventTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
+
 class ListNotificationRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
+
 class ListTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/type_defs.py` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codestar_notifications.type_defs import TargetTypeDef
 
-    data: TargetTypeDef = {...}
+    data: TargetTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -28,43 +28,43 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TargetTypeDef",
-    "CreateNotificationRuleResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
-    "DeleteNotificationRuleResultTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
     "TargetSummaryTypeDef",
     "ListEventTypesFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListNotificationRulesFilterTypeDef",
     "NotificationRuleSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "ListTargetsFilterTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubscribeResultTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResultTypeDef",
     "UnsubscribeRequestRequestTypeDef",
-    "UnsubscribeResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateNotificationRuleRequestRequestTypeDef",
     "SubscribeRequestRequestTypeDef",
     "UpdateNotificationRuleRequestRequestTypeDef",
+    "CreateNotificationRuleResultTypeDef",
+    "DeleteNotificationRuleResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "SubscribeResultTypeDef",
+    "TagResourceResultTypeDef",
+    "UnsubscribeResultTypeDef",
     "ListEventTypesResultTypeDef",
     "DescribeNotificationRuleResultTypeDef",
     "ListTargetsResultTypeDef",
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListEventTypesRequestRequestTypeDef",
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     "ListNotificationRulesRequestRequestTypeDef",
     "ListNotificationRulesResultTypeDef",
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
 )
 
@@ -73,37 +73,32 @@
     {
         "TargetType": str,
         "TargetAddress": str,
     },
     total=False,
 )
 
-CreateNotificationRuleResultTypeDef = TypedDict(
-    "CreateNotificationRuleResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteNotificationRuleRequestRequestTypeDef = TypedDict(
     "DeleteNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteNotificationRuleResultTypeDef = TypedDict(
-    "DeleteNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTargetRequestRequestTypeDef",
     {
         "TargetAddress": str,
     },
 )
 _OptionalDeleteTargetRequestRequestTypeDef = TypedDict(
@@ -153,14 +148,24 @@
     "ListEventTypesFilterTypeDef",
     {
         "Name": ListEventTypesFilterNameType,
         "Value": str,
     },
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
 ListNotificationRulesFilterTypeDef = TypedDict(
     "ListNotificationRulesFilterTypeDef",
     {
         "Name": ListNotificationRulesFilterNameType,
         "Value": str,
     },
 )
@@ -177,91 +182,38 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTargetsFilterTypeDef = TypedDict(
     "ListTargetsFilterTypeDef",
     {
         "Name": ListTargetsFilterNameType,
         "Value": str,
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
-SubscribeResultTypeDef = TypedDict(
-    "SubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagResourceResultTypeDef = TypedDict(
-    "TagResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnsubscribeRequestRequestTypeDef = TypedDict(
     "UnsubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "TargetAddress": str,
     },
 )
 
-UnsubscribeResultTypeDef = TypedDict(
-    "UnsubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -338,20 +290,68 @@
 class UpdateNotificationRuleRequestRequestTypeDef(
     _RequiredUpdateNotificationRuleRequestRequestTypeDef,
     _OptionalUpdateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
 
+CreateNotificationRuleResultTypeDef = TypedDict(
+    "CreateNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteNotificationRuleResultTypeDef = TypedDict(
+    "DeleteNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubscribeResultTypeDef = TypedDict(
+    "SubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceResultTypeDef = TypedDict(
+    "TagResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnsubscribeResultTypeDef = TypedDict(
+    "UnsubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEventTypesResultTypeDef = TypedDict(
     "ListEventTypesResultTypeDef",
     {
         "EventTypes": List[EventTypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationRuleResultTypeDef = TypedDict(
     "DescribeNotificationRuleResultTypeDef",
     {
         "Arn": str,
@@ -361,51 +361,51 @@
         "Targets": List[TargetSummaryTypeDef],
         "DetailType": DetailTypeType,
         "CreatedBy": str,
         "Status": NotificationRuleStatusType,
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResultTypeDef = TypedDict(
     "ListTargetsResultTypeDef",
     {
         "Targets": List[TargetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
+ListEventTypesRequestRequestTypeDef = TypedDict(
+    "ListEventTypesRequestRequestTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-ListEventTypesRequestRequestTypeDef = TypedDict(
-    "ListEventTypesRequestRequestTypeDef",
+ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = TypedDict(
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     {
         "Filters": Sequence[ListNotificationRulesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestRequestTypeDef = TypedDict(
     "ListNotificationRulesRequestRequestTypeDef",
     {
@@ -417,23 +417,23 @@
 )
 
 ListNotificationRulesResultTypeDef = TypedDict(
     "ListNotificationRulesResultTypeDef",
     {
         "NextToken": str,
         "NotificationRules": List[NotificationRuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
     "ListTargetsRequestListTargetsPaginateTypeDef",
     {
         "Filters": Sequence[ListTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTargetsRequestRequestTypeDef = TypedDict(
     "ListTargetsRequestRequestTypeDef",
     {
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications/type_defs.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codestar_notifications.type_defs import TargetTypeDef
 
-    data: TargetTypeDef = {...}
+    data: TargetTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -27,43 +27,43 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TargetTypeDef",
-    "CreateNotificationRuleResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
-    "DeleteNotificationRuleResultTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
     "TargetSummaryTypeDef",
     "ListEventTypesFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListNotificationRulesFilterTypeDef",
     "NotificationRuleSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "ListTargetsFilterTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubscribeResultTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResultTypeDef",
     "UnsubscribeRequestRequestTypeDef",
-    "UnsubscribeResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateNotificationRuleRequestRequestTypeDef",
     "SubscribeRequestRequestTypeDef",
     "UpdateNotificationRuleRequestRequestTypeDef",
+    "CreateNotificationRuleResultTypeDef",
+    "DeleteNotificationRuleResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "SubscribeResultTypeDef",
+    "TagResourceResultTypeDef",
+    "UnsubscribeResultTypeDef",
     "ListEventTypesResultTypeDef",
     "DescribeNotificationRuleResultTypeDef",
     "ListTargetsResultTypeDef",
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListEventTypesRequestRequestTypeDef",
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     "ListNotificationRulesRequestRequestTypeDef",
     "ListNotificationRulesResultTypeDef",
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
 )
 
@@ -72,37 +72,32 @@
     {
         "TargetType": str,
         "TargetAddress": str,
     },
     total=False,
 )
 
-CreateNotificationRuleResultTypeDef = TypedDict(
-    "CreateNotificationRuleResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteNotificationRuleRequestRequestTypeDef = TypedDict(
     "DeleteNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteNotificationRuleResultTypeDef = TypedDict(
-    "DeleteNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTargetRequestRequestTypeDef",
     {
         "TargetAddress": str,
     },
 )
 _OptionalDeleteTargetRequestRequestTypeDef = TypedDict(
@@ -150,14 +145,24 @@
     "ListEventTypesFilterTypeDef",
     {
         "Name": ListEventTypesFilterNameType,
         "Value": str,
     },
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
 ListNotificationRulesFilterTypeDef = TypedDict(
     "ListNotificationRulesFilterTypeDef",
     {
         "Name": ListNotificationRulesFilterNameType,
         "Value": str,
     },
 )
@@ -174,91 +179,38 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTargetsFilterTypeDef = TypedDict(
     "ListTargetsFilterTypeDef",
     {
         "Name": ListTargetsFilterNameType,
         "Value": str,
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
-SubscribeResultTypeDef = TypedDict(
-    "SubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagResourceResultTypeDef = TypedDict(
-    "TagResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnsubscribeRequestRequestTypeDef = TypedDict(
     "UnsubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "TargetAddress": str,
     },
 )
 
-UnsubscribeResultTypeDef = TypedDict(
-    "UnsubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -329,20 +281,68 @@
 
 class UpdateNotificationRuleRequestRequestTypeDef(
     _RequiredUpdateNotificationRuleRequestRequestTypeDef,
     _OptionalUpdateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
+CreateNotificationRuleResultTypeDef = TypedDict(
+    "CreateNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteNotificationRuleResultTypeDef = TypedDict(
+    "DeleteNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubscribeResultTypeDef = TypedDict(
+    "SubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceResultTypeDef = TypedDict(
+    "TagResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnsubscribeResultTypeDef = TypedDict(
+    "UnsubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEventTypesResultTypeDef = TypedDict(
     "ListEventTypesResultTypeDef",
     {
         "EventTypes": List[EventTypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationRuleResultTypeDef = TypedDict(
     "DescribeNotificationRuleResultTypeDef",
     {
         "Arn": str,
@@ -352,51 +352,51 @@
         "Targets": List[TargetSummaryTypeDef],
         "DetailType": DetailTypeType,
         "CreatedBy": str,
         "Status": NotificationRuleStatusType,
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResultTypeDef = TypedDict(
     "ListTargetsResultTypeDef",
     {
         "Targets": List[TargetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
+ListEventTypesRequestRequestTypeDef = TypedDict(
+    "ListEventTypesRequestRequestTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-ListEventTypesRequestRequestTypeDef = TypedDict(
-    "ListEventTypesRequestRequestTypeDef",
+ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = TypedDict(
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     {
         "Filters": Sequence[ListNotificationRulesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestRequestTypeDef = TypedDict(
     "ListNotificationRulesRequestRequestTypeDef",
     {
@@ -408,23 +408,23 @@
 )
 
 ListNotificationRulesResultTypeDef = TypedDict(
     "ListNotificationRulesResultTypeDef",
     {
         "NextToken": str,
         "NotificationRules": List[NotificationRuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
     "ListTargetsRequestListTargetsPaginateTypeDef",
     {
         "Filters": Sequence[ListTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTargetsRequestRequestTypeDef = TypedDict(
     "ListTargetsRequestRequestTypeDef",
     {
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar-notifications type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codestar-notifications type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar-notifications"></a>
 
 # types-aiobotocore-codestar-notifications
 
 [![PyPI - types-aiobotocore-codestar-notifications](https://img.shields.io/pypi/v/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar-notifications?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar-notifications)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStarNotifications 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
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
@@ -321,62 +320,63 @@
 )
 
 
 def check_value(value: DetailTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar_notifications.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_codestar_notifications.type_defs import (
     TargetTypeDef,
-    CreateNotificationRuleResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
-    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
+    CreateNotificationRuleResultTypeDef,
+    DeleteNotificationRuleResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    SubscribeResultTypeDef,
+    TagResourceResultTypeDef,
+    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListEventTypesRequestRequestTypeDef,
+    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TargetTypeDef:
+def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*


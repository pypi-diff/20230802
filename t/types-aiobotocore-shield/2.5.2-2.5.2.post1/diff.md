# Comparing `tmp/types-aiobotocore-shield-2.5.2.tar.gz` & `tmp/types-aiobotocore-shield-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-shield-2.5.2.tar", last modified: Sat Jul  8 01:44:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-shield-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
```

## Comparing `types-aiobotocore-shield-2.5.2.tar` & `types-aiobotocore-shield-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.090906 types-aiobotocore-shield-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-07-08 01:44:20.086906 types-aiobotocore-shield-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:20.090906 types-aiobotocore-shield-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.074905 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27434 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-07-08 01:41:08.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:05.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.086906 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-07-08 01:44:19.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:44:19.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:19.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:44:19.000000 types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.689455 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27464 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-shield-2.5.2/LICENSE` & `types-aiobotocore-shield-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2/PKG-INFO` & `types-aiobotocore-shield-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore shield type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore shield type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-shield"></a>
 
 # types-aiobotocore-shield
 
 [![PyPI - types-aiobotocore-shield](https://img.shields.io/pypi/v/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-shield?color=blue)](https://pypistats.org/packages/types-aiobotocore-shield)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Shield 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
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
@@ -316,99 +315,104 @@
 )
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_shield.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_shield.type_defs import (
-    ResponseActionTypeDef,
+    ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    CreateProtectionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    DescribeDRTAccessResponseTypeDef,
+    TimeRangeOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
-    GetSubscriptionStateResponseTypeDef,
+    ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
+    PaginatorConfigTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
+    CreateProtectionResponseTypeDef,
+    DescribeDRTAccessResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
+    GetSubscriptionStateResponseTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    ResponseActionUnionTypeDef,
+    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
+    TimeRangeTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     DescribeProtectionResponseTypeDef,
     ListProtectionsResponseTypeDef,
     AttackDetailTypeDef,
     DescribeAttackStatisticsResponseTypeDef,
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionTypeDef:
+def get_value() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-shield-2.5.2/README.md` & `types-aiobotocore-shield-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-shield"></a>
 
 # types-aiobotocore-shield
 
 [![PyPI - types-aiobotocore-shield](https://img.shields.io/pypi/v/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-shield?color=blue)](https://pypistats.org/packages/types-aiobotocore-shield)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Shield 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
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
@@ -283,99 +283,104 @@
 )
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_shield.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_shield.type_defs import (
-    ResponseActionTypeDef,
+    ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    CreateProtectionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    DescribeDRTAccessResponseTypeDef,
+    TimeRangeOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
-    GetSubscriptionStateResponseTypeDef,
+    ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
+    PaginatorConfigTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
+    CreateProtectionResponseTypeDef,
+    DescribeDRTAccessResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
+    GetSubscriptionStateResponseTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    ResponseActionUnionTypeDef,
+    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
+    TimeRangeTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     DescribeProtectionResponseTypeDef,
     ListProtectionsResponseTypeDef,
     AttackDetailTypeDef,
     DescribeAttackStatisticsResponseTypeDef,
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionTypeDef:
+def get_value() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-shield-2.5.2/setup.py` & `types-aiobotocore-shield-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-shield",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        " 7.17.1"
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
-    keywords="aiobotocore shield type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore shield type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_shield": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/"
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/__init__.py` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/__init__.pyi` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/__main__.py` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Shield 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Shield 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/client.py` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ResponseActionTypeDef,
+    ResponseActionUnionTypeDef,
     TagTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -332,15 +332,15 @@
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#disassociate_health_check)
         """
 
     async def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#enable_application_layer_automatic_response)
@@ -378,16 +378,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#get_subscription_state)
         """
 
     async def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -457,15 +457,15 @@
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#untag_resource)
         """
 
     async def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#update_application_layer_automatic_response)
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/client.pyi` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ResponseActionTypeDef,
+    ResponseActionUnionTypeDef,
     TagTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -303,15 +303,15 @@
         Removes health-based detection from the Shield Advanced protection for a
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#disassociate_health_check)
         """
     async def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#enable_application_layer_automatic_response)
@@ -345,16 +345,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.get_subscription_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#get_subscription_state)
         """
     async def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -417,15 +417,15 @@
         """
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#untag_resource)
         """
     async def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#update_application_layer_automatic_response)
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/literals.py` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/literals.pyi` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/paginator.py` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,59 +28,55 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAttacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
         """
 
-
 class ListProtectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/paginator.pyi` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,55 +28,59 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAttacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
         """
 
+
 class ListProtectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/type_defs.py` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for shield service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_shield.type_defs import ResponseActionTypeDef
+    from types_aiobotocore_shield.type_defs import ResponseActionOutputTypeDef
 
-    data: ResponseActionTypeDef = {...}
+    data: ResponseActionOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationLayerAutomaticResponseStatusType,
     AttackLayerType,
     AttackPropertyIdentifierType,
     AutoRenewType,
     ProactiveEngagementStatusType,
@@ -32,90 +32,95 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseActionTypeDef",
+    "ResponseActionOutputTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
-    "CreateProtectionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
-    "TimeRangeTypeDef",
-    "DescribeDRTAccessResponseTypeDef",
+    "TimeRangeOutputTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
-    "GetSubscriptionStateResponseTypeDef",
+    "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
+    "PaginatorConfigTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
-    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
+    "CreateProtectionResponseTypeDef",
+    "DescribeDRTAccessResponseTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    "GetSubscriptionStateResponseTypeDef",
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "ResponseActionUnionTypeDef",
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
+    "TimeRangeTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    "ListAttacksRequestRequestTypeDef",
+    "TimeRangeUnionTypeDef",
     "DescribeProtectionResponseTypeDef",
     "ListProtectionsResponseTypeDef",
     "AttackDetailTypeDef",
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
     "DescribeSubscriptionResponseTypeDef",
 )
 
-ResponseActionTypeDef = TypedDict(
-    "ResponseActionTypeDef",
+ResponseActionOutputTypeDef = TypedDict(
+    "ResponseActionOutputTypeDef",
     {
         "Block": Dict[str, Any],
         "Count": Dict[str, Any],
     },
     total=False,
 )
 
@@ -210,19 +215,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateProtectionResponseTypeDef = TypedDict(
-    "CreateProtectionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProtectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteProtectionGroupRequestRequestTypeDef = TypedDict(
     "DeleteProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
@@ -239,32 +247,23 @@
 DescribeAttackRequestRequestTypeDef = TypedDict(
     "DescribeAttackRequestRequestTypeDef",
     {
         "AttackId": str,
     },
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
+TimeRangeOutputTypeDef = TypedDict(
+    "TimeRangeOutputTypeDef",
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
-DescribeDRTAccessResponseTypeDef = TypedDict(
-    "DescribeDRTAccessResponseTypeDef",
-    {
-        "RoleArn": str,
-        "LogBucketList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -318,20 +317,21 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
-GetSubscriptionStateResponseTypeDef = TypedDict(
-    "GetSubscriptionStateResponseTypeDef",
+ResponseActionTypeDef = TypedDict(
+    "ResponseActionTypeDef",
     {
-        "SubscriptionState": SubscriptionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Block": Mapping[str, Any],
+        "Count": Mapping[str, Any],
     },
+    total=False,
 )
 
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
@@ -356,14 +356,24 @@
     {
         "Type": str,
         "Max": int,
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
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -379,58 +389,29 @@
 class ListResourcesInProtectionGroupRequestRequestTypeDef(
     _RequiredListResourcesInProtectionGroupRequestRequestTypeDef,
     _OptionalListResourcesInProtectionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
-    "ListResourcesInProtectionGroupResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
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
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -468,49 +449,25 @@
     total=False,
 )
 
 ApplicationLayerAutomaticResponseConfigurationTypeDef = TypedDict(
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     {
         "Status": ApplicationLayerAutomaticResponseStatusType,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
+        "Action": ResponseActionOutputTypeDef,
     },
 )
 
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
 )
 
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    {
-        "EmergencyContactList": List[EmergencyContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEmergencyContactSettingsRequestRequestTypeDef = TypedDict(
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
     total=False,
 )
@@ -614,77 +571,104 @@
 
 class CreateProtectionRequestRequestTypeDef(
     _RequiredCreateProtectionRequestRequestTypeDef, _OptionalCreateProtectionRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
+CreateProtectionResponseTypeDef = TypedDict(
+    "CreateProtectionResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ProtectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
+DescribeDRTAccessResponseTypeDef = TypedDict(
+    "DescribeDRTAccessResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
+        "RoleArn": str,
+        "LogBucketList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionStateResponseTypeDef = TypedDict(
+    "GetSubscriptionStateResponseTypeDef",
+    {
+        "SubscriptionState": SubscriptionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    {
+        "ResourceArns": List[str],
         "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionGroupsResponseTypeDef = TypedDict(
     "ListProtectionGroupsResponseTypeDef",
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
-        "InclusionFilters": InclusionProtectionFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+ResponseActionUnionTypeDef = Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
+UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
     },
-    total=False,
 )
 
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -706,21 +690,39 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
+ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    {
+        "InclusionFilters": InclusionProtectionFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "FromInclusive": TimestampTypeDef,
+        "ToExclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
 ProtectionTypeDef = TypedDict(
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
@@ -744,15 +746,15 @@
 )
 
 ListAttacksResponseTypeDef = TypedDict(
     "ListAttacksResponseTypeDef",
     {
         "AttackSummaries": List[AttackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAttackStatisticsDataItemTypeDef = TypedDict(
     "_RequiredAttackStatisticsDataItemTypeDef",
     {
         "AttackCount": int,
@@ -777,28 +779,52 @@
     "ProtectionGroupLimitsTypeDef",
     {
         "MaxProtectionGroups": int,
         "PatternTypeLimits": ProtectionGroupPatternTypeLimitsTypeDef,
     },
 )
 
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionsResponseTypeDef = TypedDict(
     "ListProtectionsResponseTypeDef",
     {
         "Protections": List[ProtectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttackDetailTypeDef = TypedDict(
     "AttackDetailTypeDef",
     {
         "AttackId": str,
@@ -812,17 +838,17 @@
     },
     total=False,
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
-        "TimeRange": TimeRangeTypeDef,
+        "TimeRange": TimeRangeOutputTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
     {
         "ProtectionLimits": ProtectionLimitsTypeDef,
@@ -830,15 +856,15 @@
     },
 )
 
 DescribeAttackResponseTypeDef = TypedDict(
     "DescribeAttackResponseTypeDef",
     {
         "Attack": AttackDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubscriptionTypeDef = TypedDict(
     "_RequiredSubscriptionTypeDef",
     {
         "SubscriptionLimits": SubscriptionLimitsTypeDef,
@@ -863,10 +889,10 @@
     pass
 
 
 DescribeSubscriptionResponseTypeDef = TypedDict(
     "DescribeSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield/type_defs.pyi` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for shield service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_shield.type_defs import ResponseActionTypeDef
+    from types_aiobotocore_shield.type_defs import ResponseActionOutputTypeDef
 
-    data: ResponseActionTypeDef = {...}
+    data: ResponseActionOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationLayerAutomaticResponseStatusType,
     AttackLayerType,
     AttackPropertyIdentifierType,
     AutoRenewType,
     ProactiveEngagementStatusType,
@@ -31,90 +31,95 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseActionTypeDef",
+    "ResponseActionOutputTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
-    "CreateProtectionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
-    "TimeRangeTypeDef",
-    "DescribeDRTAccessResponseTypeDef",
+    "TimeRangeOutputTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
-    "GetSubscriptionStateResponseTypeDef",
+    "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
+    "PaginatorConfigTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
-    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
+    "CreateProtectionResponseTypeDef",
+    "DescribeDRTAccessResponseTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    "GetSubscriptionStateResponseTypeDef",
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "ResponseActionUnionTypeDef",
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
+    "TimeRangeTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    "ListAttacksRequestRequestTypeDef",
+    "TimeRangeUnionTypeDef",
     "DescribeProtectionResponseTypeDef",
     "ListProtectionsResponseTypeDef",
     "AttackDetailTypeDef",
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
     "DescribeSubscriptionResponseTypeDef",
 )
 
-ResponseActionTypeDef = TypedDict(
-    "ResponseActionTypeDef",
+ResponseActionOutputTypeDef = TypedDict(
+    "ResponseActionOutputTypeDef",
     {
         "Block": Dict[str, Any],
         "Count": Dict[str, Any],
     },
     total=False,
 )
 
@@ -207,19 +212,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateProtectionResponseTypeDef = TypedDict(
-    "CreateProtectionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProtectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteProtectionGroupRequestRequestTypeDef = TypedDict(
     "DeleteProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
@@ -236,32 +244,23 @@
 DescribeAttackRequestRequestTypeDef = TypedDict(
     "DescribeAttackRequestRequestTypeDef",
     {
         "AttackId": str,
     },
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
+TimeRangeOutputTypeDef = TypedDict(
+    "TimeRangeOutputTypeDef",
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
-DescribeDRTAccessResponseTypeDef = TypedDict(
-    "DescribeDRTAccessResponseTypeDef",
-    {
-        "RoleArn": str,
-        "LogBucketList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -313,20 +312,21 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
-GetSubscriptionStateResponseTypeDef = TypedDict(
-    "GetSubscriptionStateResponseTypeDef",
+ResponseActionTypeDef = TypedDict(
+    "ResponseActionTypeDef",
     {
-        "SubscriptionState": SubscriptionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Block": Mapping[str, Any],
+        "Count": Mapping[str, Any],
     },
+    total=False,
 )
 
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
@@ -351,14 +351,24 @@
     {
         "Type": str,
         "Max": int,
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
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -372,58 +382,29 @@
 
 class ListResourcesInProtectionGroupRequestRequestTypeDef(
     _RequiredListResourcesInProtectionGroupRequestRequestTypeDef,
     _OptionalListResourcesInProtectionGroupRequestRequestTypeDef,
 ):
     pass
 
-ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
-    "ListResourcesInProtectionGroupResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
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
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -459,49 +440,25 @@
     total=False,
 )
 
 ApplicationLayerAutomaticResponseConfigurationTypeDef = TypedDict(
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     {
         "Status": ApplicationLayerAutomaticResponseStatusType,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
+        "Action": ResponseActionOutputTypeDef,
     },
 )
 
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
 )
 
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    {
-        "EmergencyContactList": List[EmergencyContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEmergencyContactSettingsRequestRequestTypeDef = TypedDict(
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
     total=False,
 )
@@ -599,77 +556,104 @@
 )
 
 class CreateProtectionRequestRequestTypeDef(
     _RequiredCreateProtectionRequestRequestTypeDef, _OptionalCreateProtectionRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
+CreateProtectionResponseTypeDef = TypedDict(
+    "CreateProtectionResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ProtectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
+DescribeDRTAccessResponseTypeDef = TypedDict(
+    "DescribeDRTAccessResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
+        "RoleArn": str,
+        "LogBucketList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionStateResponseTypeDef = TypedDict(
+    "GetSubscriptionStateResponseTypeDef",
+    {
+        "SubscriptionState": SubscriptionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    {
+        "ResourceArns": List[str],
         "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionGroupsResponseTypeDef = TypedDict(
     "ListProtectionGroupsResponseTypeDef",
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
-        "InclusionFilters": InclusionProtectionFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+ResponseActionUnionTypeDef = Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
+UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
     },
-    total=False,
 )
 
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -691,21 +675,39 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
+ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    {
+        "InclusionFilters": InclusionProtectionFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "FromInclusive": TimestampTypeDef,
+        "ToExclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
 ProtectionTypeDef = TypedDict(
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
@@ -729,15 +731,15 @@
 )
 
 ListAttacksResponseTypeDef = TypedDict(
     "ListAttacksResponseTypeDef",
     {
         "AttackSummaries": List[AttackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAttackStatisticsDataItemTypeDef = TypedDict(
     "_RequiredAttackStatisticsDataItemTypeDef",
     {
         "AttackCount": int,
@@ -760,28 +762,52 @@
     "ProtectionGroupLimitsTypeDef",
     {
         "MaxProtectionGroups": int,
         "PatternTypeLimits": ProtectionGroupPatternTypeLimitsTypeDef,
     },
 )
 
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionsResponseTypeDef = TypedDict(
     "ListProtectionsResponseTypeDef",
     {
         "Protections": List[ProtectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttackDetailTypeDef = TypedDict(
     "AttackDetailTypeDef",
     {
         "AttackId": str,
@@ -795,17 +821,17 @@
     },
     total=False,
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
-        "TimeRange": TimeRangeTypeDef,
+        "TimeRange": TimeRangeOutputTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
     {
         "ProtectionLimits": ProtectionLimitsTypeDef,
@@ -813,15 +839,15 @@
     },
 )
 
 DescribeAttackResponseTypeDef = TypedDict(
     "DescribeAttackResponseTypeDef",
     {
         "Attack": AttackDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubscriptionTypeDef = TypedDict(
     "_RequiredSubscriptionTypeDef",
     {
         "SubscriptionLimits": SubscriptionLimitsTypeDef,
@@ -844,10 +870,10 @@
 class SubscriptionTypeDef(_RequiredSubscriptionTypeDef, _OptionalSubscriptionTypeDef):
     pass
 
 DescribeSubscriptionResponseTypeDef = TypedDict(
     "DescribeSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/PKG-INFO` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore shield type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore shield type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-shield"></a>
 
 # types-aiobotocore-shield
 
 [![PyPI - types-aiobotocore-shield](https://img.shields.io/pypi/v/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-shield?color=blue)](https://pypistats.org/packages/types-aiobotocore-shield)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Shield 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
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
@@ -316,99 +315,104 @@
 )
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_shield.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_shield.type_defs import (
-    ResponseActionTypeDef,
+    ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    CreateProtectionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    DescribeDRTAccessResponseTypeDef,
+    TimeRangeOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
-    GetSubscriptionStateResponseTypeDef,
+    ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
+    PaginatorConfigTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
+    CreateProtectionResponseTypeDef,
+    DescribeDRTAccessResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
+    GetSubscriptionStateResponseTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    ResponseActionUnionTypeDef,
+    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
+    TimeRangeTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     DescribeProtectionResponseTypeDef,
     ListProtectionsResponseTypeDef,
     AttackDetailTypeDef,
     DescribeAttackStatisticsResponseTypeDef,
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionTypeDef:
+def get_value() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-shield-2.5.2/types_aiobotocore_shield.egg-info/SOURCES.txt` & `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*


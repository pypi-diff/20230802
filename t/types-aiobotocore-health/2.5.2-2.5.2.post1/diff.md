# Comparing `tmp/types-aiobotocore-health-2.5.2.tar.gz` & `tmp/types-aiobotocore-health-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-health-2.5.2.tar", last modified: Sat Jul  8 01:43:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-health-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
```

## Comparing `types-aiobotocore-health-2.5.2.tar` & `types-aiobotocore-health-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.298220 types-aiobotocore-health-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-08 01:43:42.298220 types-aiobotocore-health-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:42.298220 types-aiobotocore-health-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.282219 types-aiobotocore-health-2.5.2/types_aiobotocore_health/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21673 2023-07-08 01:31:56.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-08 01:31:56.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:55.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.298220 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-08 01:43:42.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:43:42.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:42.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:42.000000 types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.989575 types-aiobotocore-health-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-08-02 14:52:21.989575 types-aiobotocore-health-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.989575 types-aiobotocore-health-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.985575 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-08-02 14:39:55.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:54.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.989575 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-08-02 14:52:21.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:52:21.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:21.000000 types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-health-2.5.2/LICENSE` & `types-aiobotocore-health-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/PKG-INFO` & `types-aiobotocore-health-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-health
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore health type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore health type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-health"></a>
 
 # types-aiobotocore-health
 
 [![PyPI - types-aiobotocore-health](https://img.shields.io/pypi/v/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-health?color=blue)](https://pypistats.org/packages/types-aiobotocore-health)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Health 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [types-aiobotocore-health docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/).
 
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
@@ -341,76 +340,77 @@
 )
 
 
 def check_value(value: DescribeAffectedAccountsForOrganizationPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_health.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_health.type_defs import (
     AffectedEntityTypeDef,
-    DateTimeRangeTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    TimestampTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DateTimeRangeTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesResponseTypeDef,
-    EntityFilterTypeDef,
-    EventFilterTypeDef,
-    OrganizationEventFilterTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
     DescribeEventTypesRequestRequestTypeDef,
     DescribeEventTypesResponseTypeDef,
     DescribeEventsForOrganizationResponseTypeDef,
     DescribeEventsResponseTypeDef,
     EventDetailsTypeDef,
     OrganizationEventDetailsTypeDef,
+    EntityFilterTypeDef,
+    EventFilterTypeDef,
+    OrganizationEventFilterTypeDef,
+    DescribeEventDetailsResponseTypeDef,
+    DescribeEventDetailsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     DescribeAffectedEntitiesRequestRequestTypeDef,
     DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     DescribeEventAggregatesRequestRequestTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef,
     DescribeEventsForOrganizationRequestRequestTypeDef,
-    DescribeEventDetailsResponseTypeDef,
-    DescribeEventDetailsForOrganizationResponseTypeDef,
 )
 
 
-def get_structure() -> AffectedEntityTypeDef:
+def get_value() -> AffectedEntityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-health-2.5.2/README.md` & `types-aiobotocore-health-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-health"></a>
 
 # types-aiobotocore-health
 
 [![PyPI - types-aiobotocore-health](https://img.shields.io/pypi/v/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-health?color=blue)](https://pypistats.org/packages/types-aiobotocore-health)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Health 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [types-aiobotocore-health docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/).
 
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
@@ -308,76 +308,77 @@
 )
 
 
 def check_value(value: DescribeAffectedAccountsForOrganizationPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_health.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_health.type_defs import (
     AffectedEntityTypeDef,
-    DateTimeRangeTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    TimestampTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DateTimeRangeTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesResponseTypeDef,
-    EntityFilterTypeDef,
-    EventFilterTypeDef,
-    OrganizationEventFilterTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
     DescribeEventTypesRequestRequestTypeDef,
     DescribeEventTypesResponseTypeDef,
     DescribeEventsForOrganizationResponseTypeDef,
     DescribeEventsResponseTypeDef,
     EventDetailsTypeDef,
     OrganizationEventDetailsTypeDef,
+    EntityFilterTypeDef,
+    EventFilterTypeDef,
+    OrganizationEventFilterTypeDef,
+    DescribeEventDetailsResponseTypeDef,
+    DescribeEventDetailsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     DescribeAffectedEntitiesRequestRequestTypeDef,
     DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     DescribeEventAggregatesRequestRequestTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef,
     DescribeEventsForOrganizationRequestRequestTypeDef,
-    DescribeEventDetailsResponseTypeDef,
-    DescribeEventDetailsForOrganizationResponseTypeDef,
 )
 
 
-def get_structure() -> AffectedEntityTypeDef:
+def get_value() -> AffectedEntityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-health-2.5.2/setup.py` & `types-aiobotocore-health-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-health",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore health type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore health type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_health": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/"
```

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/__init__.py` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/__init__.pyi` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/__main__.py` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Health 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Health 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
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

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/client.py` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/client.pyi` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/literals.py` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/literals.pyi` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/paginator.py` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 class DescribeAffectedAccountsForOrganizationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, eventArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, eventArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedaccountsfororganizationpaginator)
         """
 
 
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiespaginator)
         """
 
 
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef],
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 
@@ -141,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventaggregatespaginator)
         """
 
 
@@ -160,15 +160,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventtypespaginator)
         """
 
 
@@ -179,15 +179,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventspaginator)
         """
 
 
@@ -198,13 +198,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/paginator.pyi` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 class DescribeAffectedAccountsForOrganizationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, eventArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, eventArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedaccountsfororganizationpaginator)
         """
 
 class DescribeAffectedEntitiesPaginator(AioPaginator):
@@ -98,15 +98,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiespaginator)
         """
 
 class DescribeAffectedEntitiesForOrganizationPaginator(AioPaginator):
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef],
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 class DescribeEventAggregatesPaginator(AioPaginator):
@@ -134,15 +134,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventaggregatespaginator)
         """
 
 class DescribeEventTypesPaginator(AioPaginator):
@@ -152,15 +152,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventtypespaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -170,15 +170,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventspaginator)
         """
 
 class DescribeEventsForOrganizationPaginator(AioPaginator):
@@ -188,13 +188,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/type_defs.py` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_health.type_defs import AffectedEntityTypeDef
 
-    data: AffectedEntityTypeDef = {...}
+    data: AffectedEntityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,62 +30,63 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AffectedEntityTypeDef",
-    "DateTimeRangeTypeDef",
-    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "TimestampTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
     "EventAggregateTypeDef",
     "OrganizationEventDetailsErrorItemTypeDef",
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "DateTimeRangeTypeDef",
+    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesResponseTypeDef",
-    "EntityFilterTypeDef",
-    "EventFilterTypeDef",
-    "OrganizationEventFilterTypeDef",
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     "DescribeEventDetailsForOrganizationRequestRequestTypeDef",
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     "DescribeEntityAggregatesResponseTypeDef",
     "DescribeEventAggregatesResponseTypeDef",
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     "DescribeEventTypesRequestRequestTypeDef",
     "DescribeEventTypesResponseTypeDef",
     "DescribeEventsForOrganizationResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "EventDetailsTypeDef",
     "OrganizationEventDetailsTypeDef",
+    "EntityFilterTypeDef",
+    "EventFilterTypeDef",
+    "OrganizationEventFilterTypeDef",
+    "DescribeEventDetailsResponseTypeDef",
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     "DescribeAffectedEntitiesRequestRequestTypeDef",
     "DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     "DescribeEventAggregatesRequestRequestTypeDef",
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     "DescribeEventsForOrganizationRequestRequestTypeDef",
-    "DescribeEventDetailsResponseTypeDef",
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
 )
 
 AffectedEntityTypeDef = TypedDict(
     "AffectedEntityTypeDef",
     {
         "entityArn": str,
         "eventArn": str,
@@ -95,45 +96,25 @@
         "lastUpdatedTime": datetime,
         "statusCode": entityStatusCodeType,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-DateTimeRangeTypeDef = TypedDict(
-    "DateTimeRangeTypeDef",
-    {
-        "from": Union[datetime, str],
-        "to": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "eventArn": str,
-    },
-)
-_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+TimestampTypeDef = Union[datetime, str]
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
 
-
-class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
-    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     {
         "eventArn": str,
     },
 )
 _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
@@ -149,21 +130,22 @@
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "affectedAccounts": List[str],
-        "eventScopeCode": eventScopeCodeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEventAccountFilterTypeDef = TypedDict(
     "_RequiredEventAccountFilterTypeDef",
     {
         "eventArn": str,
@@ -315,139 +297,98 @@
         "lastUpdatedTime": datetime,
         "statusCode": eventStatusCodeType,
         "eventScopeCode": eventScopeCodeType,
     },
     total=False,
 )
 
-DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+EventDescriptionTypeDef = TypedDict(
+    "EventDescriptionTypeDef",
     {
-        "healthServiceAccessStatusForOrganization": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "latestDescription": str,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+DateTimeRangeTypeDef = TypedDict(
+    "DateTimeRangeTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "from": TimestampTypeDef,
+        "to": TimestampTypeDef,
     },
+    total=False,
 )
 
-EventDescriptionTypeDef = TypedDict(
-    "EventDescriptionTypeDef",
+_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
-        "latestDescription": str,
+        "eventArn": str,
     },
-    total=False,
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
+    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+):
+    pass
+
+
+DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "affectedAccounts": List[str],
+        "eventScopeCode": eventScopeCodeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAffectedEntitiesResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredEntityFilterTypeDef = TypedDict(
-    "_RequiredEntityFilterTypeDef",
-    {
-        "eventArns": Sequence[str],
-    },
-)
-_OptionalEntityFilterTypeDef = TypedDict(
-    "_OptionalEntityFilterTypeDef",
-    {
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "tags": Sequence[Mapping[str, str]],
-        "statusCodes": Sequence[entityStatusCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
-    pass
-
-
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
+DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
     {
-        "eventArns": Sequence[str],
-        "eventTypeCodes": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "availabilityZones": Sequence[str],
-        "startTimes": Sequence[DateTimeRangeTypeDef],
-        "endTimes": Sequence[DateTimeRangeTypeDef],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "tags": Sequence[Mapping[str, str]],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
+        "healthServiceAccessStatusForOrganization": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-OrganizationEventFilterTypeDef = TypedDict(
-    "OrganizationEventFilterTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "eventTypeCodes": Sequence[str],
-        "awsAccountIds": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "startTime": DateTimeRangeTypeDef,
-        "endTime": DateTimeRangeTypeDef,
-        "lastUpdatedTime": DateTimeRangeTypeDef,
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
@@ -504,41 +445,41 @@
 
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityAggregatesResponseTypeDef = TypedDict(
     "DescribeEntityAggregatesResponseTypeDef",
     {
         "entityAggregates": List[EntityAggregateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventAggregatesResponseTypeDef = TypedDict(
     "DescribeEventAggregatesResponseTypeDef",
     {
         "eventAggregates": List[EventAggregateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = TypedDict(
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     {
         "filter": EventTypeFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventTypesRequestRequestTypeDef = TypedDict(
     "DescribeEventTypesRequestRequestTypeDef",
     {
@@ -551,33 +492,33 @@
 )
 
 DescribeEventTypesResponseTypeDef = TypedDict(
     "DescribeEventTypesResponseTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventsForOrganizationResponseTypeDef",
     {
         "events": List[OrganizationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDetailsTypeDef = TypedDict(
     "EventDetailsTypeDef",
     {
         "event": EventTypeDef,
@@ -594,25 +535,104 @@
         "event": EventTypeDef,
         "eventDescription": EventDescriptionTypeDef,
         "eventMetadata": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredEntityFilterTypeDef = TypedDict(
+    "_RequiredEntityFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+    },
+)
+_OptionalEntityFilterTypeDef = TypedDict(
+    "_OptionalEntityFilterTypeDef",
+    {
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "tags": Sequence[Mapping[str, str]],
+        "statusCodes": Sequence[entityStatusCodeType],
+    },
+    total=False,
+)
+
+
+class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
+    pass
+
+
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+        "eventTypeCodes": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "availabilityZones": Sequence[str],
+        "startTimes": Sequence[DateTimeRangeTypeDef],
+        "endTimes": Sequence[DateTimeRangeTypeDef],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "tags": Sequence[Mapping[str, str]],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+OrganizationEventFilterTypeDef = TypedDict(
+    "OrganizationEventFilterTypeDef",
+    {
+        "eventTypeCodes": Sequence[str],
+        "awsAccountIds": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "startTime": DateTimeRangeTypeDef,
+        "endTime": DateTimeRangeTypeDef,
+        "lastUpdatedTime": DateTimeRangeTypeDef,
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+DescribeEventDetailsResponseTypeDef = TypedDict(
+    "DescribeEventDetailsResponseTypeDef",
+    {
+        "successfulSet": List[EventDetailsTypeDef],
+        "failedSet": List[EventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
+    {
+        "successfulSet": List[OrganizationEventDetailsTypeDef],
+        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
@@ -651,15 +671,15 @@
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
@@ -693,15 +713,15 @@
 
 
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
@@ -714,40 +734,22 @@
 )
 
 DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsForOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestRequestTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
         "locale": str,
     },
     total=False,
 )
-
-DescribeEventDetailsResponseTypeDef = TypedDict(
-    "DescribeEventDetailsResponseTypeDef",
-    {
-        "successfulSet": List[EventDetailsTypeDef],
-        "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
-    {
-        "successfulSet": List[OrganizationEventDetailsTypeDef],
-        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health/type_defs.pyi` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_health.type_defs import AffectedEntityTypeDef
 
-    data: AffectedEntityTypeDef = {...}
+    data: AffectedEntityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -29,62 +29,63 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AffectedEntityTypeDef",
-    "DateTimeRangeTypeDef",
-    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "TimestampTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
     "EventAggregateTypeDef",
     "OrganizationEventDetailsErrorItemTypeDef",
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "DateTimeRangeTypeDef",
+    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesResponseTypeDef",
-    "EntityFilterTypeDef",
-    "EventFilterTypeDef",
-    "OrganizationEventFilterTypeDef",
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     "DescribeEventDetailsForOrganizationRequestRequestTypeDef",
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     "DescribeEntityAggregatesResponseTypeDef",
     "DescribeEventAggregatesResponseTypeDef",
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     "DescribeEventTypesRequestRequestTypeDef",
     "DescribeEventTypesResponseTypeDef",
     "DescribeEventsForOrganizationResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "EventDetailsTypeDef",
     "OrganizationEventDetailsTypeDef",
+    "EntityFilterTypeDef",
+    "EventFilterTypeDef",
+    "OrganizationEventFilterTypeDef",
+    "DescribeEventDetailsResponseTypeDef",
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     "DescribeAffectedEntitiesRequestRequestTypeDef",
     "DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     "DescribeEventAggregatesRequestRequestTypeDef",
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     "DescribeEventsForOrganizationRequestRequestTypeDef",
-    "DescribeEventDetailsResponseTypeDef",
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
 )
 
 AffectedEntityTypeDef = TypedDict(
     "AffectedEntityTypeDef",
     {
         "entityArn": str,
         "eventArn": str,
@@ -94,43 +95,25 @@
         "lastUpdatedTime": datetime,
         "statusCode": entityStatusCodeType,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-DateTimeRangeTypeDef = TypedDict(
-    "DateTimeRangeTypeDef",
-    {
-        "from": Union[datetime, str],
-        "to": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "eventArn": str,
-    },
-)
-_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+TimestampTypeDef = Union[datetime, str]
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
 
-class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
-    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     {
         "eventArn": str,
     },
 )
 _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
@@ -144,21 +127,22 @@
 
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "affectedAccounts": List[str],
-        "eventScopeCode": eventScopeCodeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEventAccountFilterTypeDef = TypedDict(
     "_RequiredEventAccountFilterTypeDef",
     {
         "eventArn": str,
@@ -306,137 +290,96 @@
         "lastUpdatedTime": datetime,
         "statusCode": eventStatusCodeType,
         "eventScopeCode": eventScopeCodeType,
     },
     total=False,
 )
 
-DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+EventDescriptionTypeDef = TypedDict(
+    "EventDescriptionTypeDef",
     {
-        "healthServiceAccessStatusForOrganization": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "latestDescription": str,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+DateTimeRangeTypeDef = TypedDict(
+    "DateTimeRangeTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "from": TimestampTypeDef,
+        "to": TimestampTypeDef,
     },
+    total=False,
 )
 
-EventDescriptionTypeDef = TypedDict(
-    "EventDescriptionTypeDef",
+_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
-        "latestDescription": str,
+        "eventArn": str,
     },
-    total=False,
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
+    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+):
+    pass
+
+DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "affectedAccounts": List[str],
+        "eventScopeCode": eventScopeCodeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAffectedEntitiesResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEntityFilterTypeDef = TypedDict(
-    "_RequiredEntityFilterTypeDef",
-    {
-        "eventArns": Sequence[str],
-    },
-)
-_OptionalEntityFilterTypeDef = TypedDict(
-    "_OptionalEntityFilterTypeDef",
-    {
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "tags": Sequence[Mapping[str, str]],
-        "statusCodes": Sequence[entityStatusCodeType],
-    },
-    total=False,
-)
-
-class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
-    pass
-
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
+DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
     {
-        "eventArns": Sequence[str],
-        "eventTypeCodes": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "availabilityZones": Sequence[str],
-        "startTimes": Sequence[DateTimeRangeTypeDef],
-        "endTimes": Sequence[DateTimeRangeTypeDef],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "tags": Sequence[Mapping[str, str]],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
+        "healthServiceAccessStatusForOrganization": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-OrganizationEventFilterTypeDef = TypedDict(
-    "OrganizationEventFilterTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "eventTypeCodes": Sequence[str],
-        "awsAccountIds": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "startTime": DateTimeRangeTypeDef,
-        "endTime": DateTimeRangeTypeDef,
-        "lastUpdatedTime": DateTimeRangeTypeDef,
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
@@ -487,41 +430,41 @@
 
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityAggregatesResponseTypeDef = TypedDict(
     "DescribeEntityAggregatesResponseTypeDef",
     {
         "entityAggregates": List[EntityAggregateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventAggregatesResponseTypeDef = TypedDict(
     "DescribeEventAggregatesResponseTypeDef",
     {
         "eventAggregates": List[EventAggregateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = TypedDict(
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     {
         "filter": EventTypeFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventTypesRequestRequestTypeDef = TypedDict(
     "DescribeEventTypesRequestRequestTypeDef",
     {
@@ -534,33 +477,33 @@
 )
 
 DescribeEventTypesResponseTypeDef = TypedDict(
     "DescribeEventTypesResponseTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventsForOrganizationResponseTypeDef",
     {
         "events": List[OrganizationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDetailsTypeDef = TypedDict(
     "EventDetailsTypeDef",
     {
         "event": EventTypeDef,
@@ -577,25 +520,102 @@
         "event": EventTypeDef,
         "eventDescription": EventDescriptionTypeDef,
         "eventMetadata": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredEntityFilterTypeDef = TypedDict(
+    "_RequiredEntityFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+    },
+)
+_OptionalEntityFilterTypeDef = TypedDict(
+    "_OptionalEntityFilterTypeDef",
+    {
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "tags": Sequence[Mapping[str, str]],
+        "statusCodes": Sequence[entityStatusCodeType],
+    },
+    total=False,
+)
+
+class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
+    pass
+
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+        "eventTypeCodes": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "availabilityZones": Sequence[str],
+        "startTimes": Sequence[DateTimeRangeTypeDef],
+        "endTimes": Sequence[DateTimeRangeTypeDef],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "tags": Sequence[Mapping[str, str]],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+OrganizationEventFilterTypeDef = TypedDict(
+    "OrganizationEventFilterTypeDef",
+    {
+        "eventTypeCodes": Sequence[str],
+        "awsAccountIds": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "startTime": DateTimeRangeTypeDef,
+        "endTime": DateTimeRangeTypeDef,
+        "lastUpdatedTime": DateTimeRangeTypeDef,
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+DescribeEventDetailsResponseTypeDef = TypedDict(
+    "DescribeEventDetailsResponseTypeDef",
+    {
+        "successfulSet": List[EventDetailsTypeDef],
+        "failedSet": List[EventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
+    {
+        "successfulSet": List[OrganizationEventDetailsTypeDef],
+        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
@@ -630,15 +650,15 @@
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
@@ -668,15 +688,15 @@
     pass
 
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
@@ -689,40 +709,22 @@
 )
 
 DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsForOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestRequestTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
         "locale": str,
     },
     total=False,
 )
-
-DescribeEventDetailsResponseTypeDef = TypedDict(
-    "DescribeEventDetailsResponseTypeDef",
-    {
-        "successfulSet": List[EventDetailsTypeDef],
-        "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
-    {
-        "successfulSet": List[OrganizationEventDetailsTypeDef],
-        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/PKG-INFO` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-health
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore health type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore health type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-health"></a>
 
 # types-aiobotocore-health
 
 [![PyPI - types-aiobotocore-health](https://img.shields.io/pypi/v/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-health?color=blue)](https://pypistats.org/packages/types-aiobotocore-health)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Health 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [types-aiobotocore-health docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/).
 
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
@@ -341,76 +340,77 @@
 )
 
 
 def check_value(value: DescribeAffectedAccountsForOrganizationPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_health.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_health.type_defs import (
     AffectedEntityTypeDef,
-    DateTimeRangeTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    TimestampTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DateTimeRangeTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesResponseTypeDef,
-    EntityFilterTypeDef,
-    EventFilterTypeDef,
-    OrganizationEventFilterTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
     DescribeEventTypesRequestRequestTypeDef,
     DescribeEventTypesResponseTypeDef,
     DescribeEventsForOrganizationResponseTypeDef,
     DescribeEventsResponseTypeDef,
     EventDetailsTypeDef,
     OrganizationEventDetailsTypeDef,
+    EntityFilterTypeDef,
+    EventFilterTypeDef,
+    OrganizationEventFilterTypeDef,
+    DescribeEventDetailsResponseTypeDef,
+    DescribeEventDetailsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     DescribeAffectedEntitiesRequestRequestTypeDef,
     DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     DescribeEventAggregatesRequestRequestTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef,
     DescribeEventsForOrganizationRequestRequestTypeDef,
-    DescribeEventDetailsResponseTypeDef,
-    DescribeEventDetailsForOrganizationResponseTypeDef,
 )
 
 
-def get_structure() -> AffectedEntityTypeDef:
+def get_value() -> AffectedEntityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-health-2.5.2/types_aiobotocore_health.egg-info/SOURCES.txt` & `types-aiobotocore-health-2.5.2.post1/types_aiobotocore_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*


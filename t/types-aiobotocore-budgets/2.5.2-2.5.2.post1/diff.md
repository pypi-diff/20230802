# Comparing `tmp/types-aiobotocore-budgets-2.5.2.tar.gz` & `tmp/types-aiobotocore-budgets-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-budgets-2.5.2.tar", last modified: Sat Jul  8 01:43:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-budgets-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-budgets-2.5.2.tar` & `types-aiobotocore-budgets-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.941776 types-aiobotocore-budgets-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-08 01:43:18.937776 types-aiobotocore-budgets-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:18.941776 types-aiobotocore-budgets-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.933776 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31392 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.937776 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.533643 types-aiobotocore-budgets-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-08-02 14:51:57.529643 types-aiobotocore-budgets-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.533643 types-aiobotocore-budgets-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:53.000000 types-aiobotocore-budgets-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.525643 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34558 2023-08-02 14:33:55.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.529643 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-budgets-2.5.2/LICENSE` & `types-aiobotocore-budgets-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2/PKG-INFO` & `types-aiobotocore-budgets-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-budgets
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore budgets type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-budgets"></a>
 
 # types-aiobotocore-budgets
 
 [![PyPI - types-aiobotocore-budgets](https://img.shields.io/pypi/v/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-budgets?color=blue)](https://pypistats.org/packages/types-aiobotocore-budgets)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [types-aiobotocore-budgets docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -354,95 +321,106 @@
 )
 
 
 def check_value(value: ActionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_budgets.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_budgets.type_defs import (
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
+    TimestampTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
-    TimePeriodTypeDef,
-    CreateBudgetActionResponseTypeDef,
+    TimePeriodOutputTypeDef,
+    ResponseMetadataTypeDef,
+    IamActionDefinitionOutputTypeDef,
+    ScpActionDefinitionOutputTypeDef,
+    SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
-    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestRequestTypeDef,
-    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestRequestTypeDef,
-    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
-    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
-    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
-    ExecuteBudgetActionResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeSubscribersForNotificationResponseTypeDef,
+    AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
+    TimePeriodTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
-    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
+    CreateBudgetActionResponseTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    DescribeSubscribersForNotificationResponseTypeDef,
+    ExecuteBudgetActionResponseTypeDef,
+    DefinitionOutputTypeDef,
+    DefinitionTypeDef,
+    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    DefinitionTypeDef,
+    TimePeriodUnionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
+    BudgetOutputTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
+    DefinitionUnionTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
-    CreateBudgetRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
+    BudgetUnionTypeDef,
+    CreateBudgetRequestRequestTypeDef,
     UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_value() -> ActionThresholdTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-budgets-2.5.2/README.md` & `types-aiobotocore-budgets-2.5.2.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-budgets
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore budgets type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-budgets"></a>
 
 # types-aiobotocore-budgets
 
 [![PyPI - types-aiobotocore-budgets](https://img.shields.io/pypi/v/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-budgets?color=blue)](https://pypistats.org/packages/types-aiobotocore-budgets)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [types-aiobotocore-budgets docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -321,95 +353,106 @@
 )
 
 
 def check_value(value: ActionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_budgets.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_budgets.type_defs import (
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
+    TimestampTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
-    TimePeriodTypeDef,
-    CreateBudgetActionResponseTypeDef,
+    TimePeriodOutputTypeDef,
+    ResponseMetadataTypeDef,
+    IamActionDefinitionOutputTypeDef,
+    ScpActionDefinitionOutputTypeDef,
+    SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
-    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestRequestTypeDef,
-    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestRequestTypeDef,
-    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
-    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
-    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
-    ExecuteBudgetActionResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeSubscribersForNotificationResponseTypeDef,
+    AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
+    TimePeriodTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
-    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
+    CreateBudgetActionResponseTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    DescribeSubscribersForNotificationResponseTypeDef,
+    ExecuteBudgetActionResponseTypeDef,
+    DefinitionOutputTypeDef,
+    DefinitionTypeDef,
+    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    DefinitionTypeDef,
+    TimePeriodUnionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
+    BudgetOutputTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
+    DefinitionUnionTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
-    CreateBudgetRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
+    BudgetUnionTypeDef,
+    CreateBudgetRequestRequestTypeDef,
     UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_value() -> ActionThresholdTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-budgets-2.5.2/setup.py` & `types-aiobotocore-budgets-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-budgets",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore budgets type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore budgets type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_budgets": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/"
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.py` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.pyi` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__main__.py` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Budgets 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Budgets 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.py` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionTypeDef,
+    DefinitionUnionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
@@ -47,15 +47,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -119,15 +119,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#close)
         """
 
     async def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetTypeDef,
+        Budget: BudgetUnionTypeDef,
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget)
@@ -137,15 +137,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionTypeDef,
+        Definition: DefinitionUnionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -248,15 +248,15 @@
 
     async def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -294,15 +294,15 @@
         """
 
     async def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -365,15 +365,17 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#generate_presigned_url)
         """
 
-    async def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
+    async def update_budget(
+        self, *, AccountId: str, NewBudget: BudgetUnionTypeDef
+    ) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_budget)
         """
 
@@ -381,15 +383,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionTypeDef = ...,
+        Definition: DefinitionUnionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.pyi` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionTypeDef,
+    DefinitionUnionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
@@ -47,15 +47,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -112,15 +112,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#close)
         """
     async def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetTypeDef,
+        Budget: BudgetUnionTypeDef,
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget)
@@ -129,15 +129,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionTypeDef,
+        Definition: DefinitionUnionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -231,15 +231,15 @@
         """
     async def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -273,15 +273,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_budget_notifications_for_account)
         """
     async def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -338,30 +338,32 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#generate_presigned_url)
         """
-    async def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
+    async def update_budget(
+        self, *, AccountId: str, NewBudget: BudgetUnionTypeDef
+    ) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_budget)
         """
     async def update_budget_action(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionTypeDef = ...,
+        Definition: DefinitionUnionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.py` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.pyi` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.py` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -83,61 +83,61 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
 
 class DescribeBudgetActionsForAccountPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforaccountpaginator)
         """
 
 
 class DescribeBudgetActionsForBudgetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforbudgetpaginator)
         """
 
 
 class DescribeBudgetNotificationsForAccountPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
         """
 
 
@@ -148,46 +148,46 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
 
 class DescribeBudgetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetspaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetspaginator)
         """
 
 
 class DescribeNotificationsForBudgetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describenotificationsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeNotificationsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describenotificationsforbudgetpaginator)
         """
 
 
@@ -199,13 +199,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.pyi` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -80,58 +80,58 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
 class DescribeBudgetActionsForAccountPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforaccountpaginator)
         """
 
 class DescribeBudgetActionsForBudgetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionsforbudgetpaginator)
         """
 
 class DescribeBudgetNotificationsForAccountPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
         """
 
 class DescribeBudgetPerformanceHistoryPaginator(AioPaginator):
@@ -141,44 +141,44 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
 class DescribeBudgetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetspaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetspaginator)
         """
 
 class DescribeNotificationsForBudgetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describenotificationsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeNotificationsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describenotificationsforbudgetpaginator)
         """
 
 class DescribeSubscribersForNotificationPaginator(AioPaginator):
@@ -189,13 +189,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.py` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_budgets.type_defs import ActionThresholdTypeDef
 
-    data: ActionThresholdTypeDef = {...}
+    data: ActionThresholdTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,74 +33,84 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
+    "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
-    "TimePeriodTypeDef",
-    "CreateBudgetActionResponseTypeDef",
+    "TimePeriodOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "IamActionDefinitionOutputTypeDef",
+    "ScpActionDefinitionOutputTypeDef",
+    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
-    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
-    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
-    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
-    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
-    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
-    "ExecuteBudgetActionResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "DescribeSubscribersForNotificationResponseTypeDef",
+    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
+    "TimePeriodTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
     "BudgetedAndActualAmountsTypeDef",
+    "CreateBudgetActionResponseTypeDef",
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    "DescribeSubscribersForNotificationResponseTypeDef",
+    "ExecuteBudgetActionResponseTypeDef",
+    "DefinitionOutputTypeDef",
+    "DefinitionTypeDef",
+    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "DefinitionTypeDef",
+    "TimePeriodUnionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
+    "BudgetOutputTypeDef",
     "BudgetTypeDef",
     "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
+    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
+    "BudgetUnionTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
@@ -135,21 +145,20 @@
     "_OptionalHistoricalOptionsTypeDef",
     {
         "LookBackAvailablePeriods": int,
     },
     total=False,
 )
 
-
 class HistoricalOptionsTypeDef(
     _RequiredHistoricalOptionsTypeDef, _OptionalHistoricalOptionsTypeDef
 ):
     pass
 
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredNotificationTypeDef = TypedDict(
     "_RequiredNotificationTypeDef",
     {
         "NotificationType": NotificationTypeType,
         "ComparisonOperator": ComparisonOperatorType,
         "Threshold": float,
     },
@@ -159,19 +168,17 @@
     {
         "ThresholdType": ThresholdTypeType,
         "NotificationState": NotificationStateType,
     },
     total=False,
 )
 
-
 class NotificationTypeDef(_RequiredNotificationTypeDef, _OptionalNotificationTypeDef):
     pass
 
-
 CostTypesTypeDef = TypedDict(
     "CostTypesTypeDef",
     {
         "IncludeTax": bool,
         "IncludeSubscription": bool,
         "UseBlended": bool,
         "IncludeRefund": bool,
@@ -190,30 +197,69 @@
     "SpendTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
 )
 
-TimePeriodTypeDef = TypedDict(
-    "TimePeriodTypeDef",
+TimePeriodOutputTypeDef = TypedDict(
+    "TimePeriodOutputTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
+        "Start": datetime,
+        "End": datetime,
     },
     total=False,
 )
 
-CreateBudgetActionResponseTypeDef = TypedDict(
-    "CreateBudgetActionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+_RequiredIamActionDefinitionOutputTypeDef = TypedDict(
+    "_RequiredIamActionDefinitionOutputTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalIamActionDefinitionOutputTypeDef = TypedDict(
+    "_OptionalIamActionDefinitionOutputTypeDef",
+    {
+        "Roles": List[str],
+        "Groups": List[str],
+        "Users": List[str],
+    },
+    total=False,
+)
+
+class IamActionDefinitionOutputTypeDef(
+    _RequiredIamActionDefinitionOutputTypeDef, _OptionalIamActionDefinitionOutputTypeDef
+):
+    pass
+
+ScpActionDefinitionOutputTypeDef = TypedDict(
+    "ScpActionDefinitionOutputTypeDef",
+    {
+        "PolicyId": str,
+        "TargetIds": List[str],
+    },
+)
+
+SsmActionDefinitionOutputTypeDef = TypedDict(
+    "SsmActionDefinitionOutputTypeDef",
+    {
+        "ActionSubType": ActionSubTypeType,
+        "Region": str,
+        "InstanceIds": List[str],
     },
 )
 
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
@@ -225,21 +271,19 @@
         "Roles": Sequence[str],
         "Groups": Sequence[str],
         "Users": Sequence[str],
     },
     total=False,
 )
 
-
 class IamActionDefinitionTypeDef(
     _RequiredIamActionDefinitionTypeDef, _OptionalIamActionDefinitionTypeDef
 ):
     pass
 
-
 ScpActionDefinitionTypeDef = TypedDict(
     "ScpActionDefinitionTypeDef",
     {
         "PolicyId": str,
         "TargetIds": Sequence[str],
     },
 )
@@ -266,44 +310,32 @@
     "DeleteBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 
-DescribeBudgetActionRequestRequestTypeDef = TypedDict(
-    "DescribeBudgetActionRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+DescribeBudgetActionRequestRequestTypeDef = TypedDict(
+    "DescribeBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
     },
 )
-_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-):
-    pass
-
 
 _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
@@ -312,45 +344,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeBudgetActionsForAccountRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForAccountRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -359,44 +366,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeBudgetActionsForBudgetRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForBudgetRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
@@ -404,52 +387,28 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeBudgetNotificationsForAccountRequestRequestTypeDef(
     _RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     _OptionalDescribeBudgetNotificationsForAccountRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeBudgetRequestRequestTypeDef = TypedDict(
     "DescribeBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 
-_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
-    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeBudgetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetsRequestRequestTypeDef = TypedDict(
@@ -457,44 +416,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeBudgetsRequestRequestTypeDef(
     _RequiredDescribeBudgetsRequestRequestTypeDef, _OptionalDescribeBudgetsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
-    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeNotificationsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -503,92 +437,76 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeNotificationsForBudgetRequestRequestTypeDef(
     _RequiredDescribeNotificationsForBudgetRequestRequestTypeDef,
     _OptionalDescribeNotificationsForBudgetRequestRequestTypeDef,
 ):
     pass
 
-
 ExecuteBudgetActionRequestRequestTypeDef = TypedDict(
     "ExecuteBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
 
-ExecuteBudgetActionResponseTypeDef = TypedDict(
-    "ExecuteBudgetActionResponseTypeDef",
+_RequiredAutoAdjustDataOutputTypeDef = TypedDict(
+    "_RequiredAutoAdjustDataOutputTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ExecutionType": ExecutionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AutoAdjustType": AutoAdjustTypeType,
     },
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalAutoAdjustDataOutputTypeDef = TypedDict(
+    "_OptionalAutoAdjustDataOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HistoricalOptions": HistoricalOptionsTypeDef,
+        "LastAutoAdjustTime": datetime,
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
-DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
-    "DescribeSubscribersForNotificationResponseTypeDef",
-    {
-        "Subscribers": List[SubscriberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class AutoAdjustDataOutputTypeDef(
+    _RequiredAutoAdjustDataOutputTypeDef, _OptionalAutoAdjustDataOutputTypeDef
+):
+    pass
 
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
     "_OptionalAutoAdjustDataTypeDef",
     {
         "HistoricalOptions": HistoricalOptionsTypeDef,
-        "LastAutoAdjustTime": Union[datetime, str],
+        "LastAutoAdjustTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class AutoAdjustDataTypeDef(_RequiredAutoAdjustDataTypeDef, _OptionalAutoAdjustDataTypeDef):
     pass
 
+TimePeriodTypeDef = TypedDict(
+    "TimePeriodTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+    },
+    total=False,
+)
 
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
         "Notifications": List[NotificationTypeDef],
         "BudgetName": str,
     },
@@ -630,47 +548,14 @@
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "Subscriber": SubscriberTypeDef,
     },
 )
 
-DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    {
-        "Notifications": List[NotificationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
     },
@@ -680,22 +565,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeSubscribersForNotificationRequestRequestTypeDef(
     _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef,
     _OptionalDescribeSubscribersForNotificationRequestRequestTypeDef,
 ):
     pass
 
-
 NotificationWithSubscribersTypeDef = TypedDict(
     "NotificationWithSubscribersTypeDef",
     {
         "Notification": NotificationTypeDef,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
@@ -731,29 +614,210 @@
     "_OptionalCalculatedSpendTypeDef",
     {
         "ForecastedSpend": SpendTypeDef,
     },
     total=False,
 )
 
-
 class CalculatedSpendTypeDef(_RequiredCalculatedSpendTypeDef, _OptionalCalculatedSpendTypeDef):
     pass
 
-
 BudgetedAndActualAmountsTypeDef = TypedDict(
     "BudgetedAndActualAmountsTypeDef",
     {
         "BudgetedAmount": SpendTypeDef,
         "ActualAmount": SpendTypeDef,
-        "TimePeriod": TimePeriodTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
+    },
+    total=False,
+)
+
+CreateBudgetActionResponseTypeDef = TypedDict(
+    "CreateBudgetActionResponseTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    {
+        "Notifications": List[NotificationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
+    "DescribeSubscribersForNotificationResponseTypeDef",
+    {
+        "Subscribers": List[SubscriberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExecuteBudgetActionResponseTypeDef = TypedDict(
+    "ExecuteBudgetActionResponseTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ExecutionType": ExecutionTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DefinitionOutputTypeDef = TypedDict(
+    "DefinitionOutputTypeDef",
+    {
+        "IamActionDefinition": IamActionDefinitionOutputTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionOutputTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
+DefinitionTypeDef = TypedDict(
+    "DefinitionTypeDef",
+    {
+        "IamActionDefinition": IamActionDefinitionTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
+    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
+    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -761,28 +825,26 @@
     )
 )
 _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "TimePeriod": TimePeriodTypeDef,
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
-
 class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
     _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -793,46 +855,42 @@
         "TimePeriod": TimePeriodTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeBudgetActionHistoriesRequestRequestTypeDef(
     _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
     _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "TimePeriod": TimePeriodTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -842,41 +900,56 @@
         "TimePeriod": TimePeriodTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
-
-DefinitionTypeDef = TypedDict(
-    "DefinitionTypeDef",
-    {
-        "IamActionDefinition": IamActionDefinitionTypeDef,
-        "ScpActionDefinition": ScpActionDefinitionTypeDef,
-        "SsmActionDefinition": SsmActionDefinitionTypeDef,
-    },
-    total=False,
-)
-
+TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodOutputTypeDef]
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBudgetOutputTypeDef = TypedDict(
+    "_RequiredBudgetOutputTypeDef",
+    {
+        "BudgetName": str,
+        "TimeUnit": TimeUnitType,
+        "BudgetType": BudgetTypeType,
+    },
+)
+_OptionalBudgetOutputTypeDef = TypedDict(
+    "_OptionalBudgetOutputTypeDef",
+    {
+        "BudgetLimit": SpendTypeDef,
+        "PlannedBudgetLimits": Dict[str, SpendTypeDef],
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
+        "CalculatedSpend": CalculatedSpendTypeDef,
+        "LastUpdatedTime": datetime,
+        "AutoAdjustData": AutoAdjustDataOutputTypeDef,
     },
+    total=False,
 )
 
+class BudgetOutputTypeDef(_RequiredBudgetOutputTypeDef, _OptionalBudgetOutputTypeDef):
+    pass
+
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
     },
@@ -886,25 +959,23 @@
     {
         "BudgetLimit": SpendTypeDef,
         "PlannedBudgetLimits": Mapping[str, SpendTypeDef],
         "CostFilters": Mapping[str, Sequence[str]],
         "CostTypes": CostTypesTypeDef,
         "TimePeriod": TimePeriodTypeDef,
         "CalculatedSpend": CalculatedSpendTypeDef,
-        "LastUpdatedTime": Union[datetime, str],
+        "LastUpdatedTime": TimestampTypeDef,
         "AutoAdjustData": AutoAdjustDataTypeDef,
     },
     total=False,
 )
 
-
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
 
-
 BudgetPerformanceHistoryTypeDef = TypedDict(
     "BudgetPerformanceHistoryTypeDef",
     {
         "BudgetName": str,
         "BudgetType": BudgetTypeType,
         "CostFilters": Dict[str, List[str]],
         "CostTypes": CostTypesTypeDef,
@@ -918,15 +989,15 @@
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionTypeDef,
+        "Definition": DefinitionOutputTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
         "Subscribers": List[SubscriberTypeDef],
     },
 )
 
@@ -941,14 +1012,15 @@
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
 
+DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionOutputTypeDef]
 _RequiredUpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -962,22 +1034,38 @@
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
     total=False,
 )
 
-
 class UpdateBudgetActionRequestRequestTypeDef(
     _RequiredUpdateBudgetActionRequestRequestTypeDef,
     _OptionalUpdateBudgetActionRequestRequestTypeDef,
 ):
     pass
 
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
+    {
+        "Budget": BudgetOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
+    {
+        "Budgets": List[BudgetOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetOutputTypeDef]
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
@@ -985,52 +1073,33 @@
     "_OptionalCreateBudgetRequestRequestTypeDef",
     {
         "NotificationsWithSubscribers": Sequence[NotificationWithSubscribersTypeDef],
     },
     total=False,
 )
 
-
 class CreateBudgetRequestRequestTypeDef(
     _RequiredCreateBudgetRequestRequestTypeDef, _OptionalCreateBudgetRequestRequestTypeDef
 ):
     pass
 
-
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
-    {
-        "Budgets": List[BudgetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "NewBudget": BudgetTypeDef,
     },
 )
 
 DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     {
         "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
@@ -1040,54 +1109,54 @@
 
 DeleteBudgetActionResponseTypeDef = TypedDict(
     "DeleteBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBudgetActionResponseTypeDef = TypedDict(
     "DescribeBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBudgetActionsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForAccountResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBudgetActionsForBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBudgetActionResponseTypeDef = TypedDict(
     "UpdateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
@@ -1098,10 +1167,10 @@
 )
 
 DescribeBudgetActionHistoriesResponseTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesResponseTypeDef",
     {
         "ActionHistories": List[ActionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.pyi` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_budgets.type_defs import ActionThresholdTypeDef
 
-    data: ActionThresholdTypeDef = {...}
+    data: ActionThresholdTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,73 +33,85 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
+    "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
-    "TimePeriodTypeDef",
-    "CreateBudgetActionResponseTypeDef",
+    "TimePeriodOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "IamActionDefinitionOutputTypeDef",
+    "ScpActionDefinitionOutputTypeDef",
+    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
-    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
-    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
-    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
-    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
-    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
-    "ExecuteBudgetActionResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "DescribeSubscribersForNotificationResponseTypeDef",
+    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
+    "TimePeriodTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
     "BudgetedAndActualAmountsTypeDef",
+    "CreateBudgetActionResponseTypeDef",
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    "DescribeSubscribersForNotificationResponseTypeDef",
+    "ExecuteBudgetActionResponseTypeDef",
+    "DefinitionOutputTypeDef",
+    "DefinitionTypeDef",
+    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "DefinitionTypeDef",
+    "TimePeriodUnionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
+    "BudgetOutputTypeDef",
     "BudgetTypeDef",
     "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
+    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
+    "BudgetUnionTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
@@ -134,19 +146,22 @@
     "_OptionalHistoricalOptionsTypeDef",
     {
         "LookBackAvailablePeriods": int,
     },
     total=False,
 )
 
+
 class HistoricalOptionsTypeDef(
     _RequiredHistoricalOptionsTypeDef, _OptionalHistoricalOptionsTypeDef
 ):
     pass
 
+
+TimestampTypeDef = Union[datetime, str]
 _RequiredNotificationTypeDef = TypedDict(
     "_RequiredNotificationTypeDef",
     {
         "NotificationType": NotificationTypeType,
         "ComparisonOperator": ComparisonOperatorType,
         "Threshold": float,
     },
@@ -156,17 +171,19 @@
     {
         "ThresholdType": ThresholdTypeType,
         "NotificationState": NotificationStateType,
     },
     total=False,
 )
 
+
 class NotificationTypeDef(_RequiredNotificationTypeDef, _OptionalNotificationTypeDef):
     pass
 
+
 CostTypesTypeDef = TypedDict(
     "CostTypesTypeDef",
     {
         "IncludeTax": bool,
         "IncludeSubscription": bool,
         "UseBlended": bool,
         "IncludeRefund": bool,
@@ -185,30 +202,71 @@
     "SpendTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
 )
 
-TimePeriodTypeDef = TypedDict(
-    "TimePeriodTypeDef",
+TimePeriodOutputTypeDef = TypedDict(
+    "TimePeriodOutputTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
+        "Start": datetime,
+        "End": datetime,
     },
     total=False,
 )
 
-CreateBudgetActionResponseTypeDef = TypedDict(
-    "CreateBudgetActionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+_RequiredIamActionDefinitionOutputTypeDef = TypedDict(
+    "_RequiredIamActionDefinitionOutputTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalIamActionDefinitionOutputTypeDef = TypedDict(
+    "_OptionalIamActionDefinitionOutputTypeDef",
+    {
+        "Roles": List[str],
+        "Groups": List[str],
+        "Users": List[str],
+    },
+    total=False,
+)
+
+
+class IamActionDefinitionOutputTypeDef(
+    _RequiredIamActionDefinitionOutputTypeDef, _OptionalIamActionDefinitionOutputTypeDef
+):
+    pass
+
+
+ScpActionDefinitionOutputTypeDef = TypedDict(
+    "ScpActionDefinitionOutputTypeDef",
+    {
+        "PolicyId": str,
+        "TargetIds": List[str],
+    },
+)
+
+SsmActionDefinitionOutputTypeDef = TypedDict(
+    "SsmActionDefinitionOutputTypeDef",
+    {
+        "ActionSubType": ActionSubTypeType,
+        "Region": str,
+        "InstanceIds": List[str],
     },
 )
 
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
@@ -220,19 +278,21 @@
         "Roles": Sequence[str],
         "Groups": Sequence[str],
         "Users": Sequence[str],
     },
     total=False,
 )
 
+
 class IamActionDefinitionTypeDef(
     _RequiredIamActionDefinitionTypeDef, _OptionalIamActionDefinitionTypeDef
 ):
     pass
 
+
 ScpActionDefinitionTypeDef = TypedDict(
     "ScpActionDefinitionTypeDef",
     {
         "PolicyId": str,
         "TargetIds": Sequence[str],
     },
 )
@@ -259,42 +319,32 @@
     "DeleteBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 
-DescribeBudgetActionRequestRequestTypeDef = TypedDict(
-    "DescribeBudgetActionRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+DescribeBudgetActionRequestRequestTypeDef = TypedDict(
+    "DescribeBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
     },
 )
-_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
@@ -303,40 +353,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeBudgetActionsForAccountRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForAccountRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
@@ -346,39 +377,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeBudgetActionsForBudgetRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForBudgetRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
@@ -387,48 +400,30 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeBudgetNotificationsForAccountRequestRequestTypeDef(
     _RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     _OptionalDescribeBudgetNotificationsForAccountRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeBudgetRequestRequestTypeDef = TypedDict(
     "DescribeBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 
-_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
-    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeBudgetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetsRequestRequestTypeDef = TypedDict(
@@ -436,39 +431,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeBudgetsRequestRequestTypeDef(
     _RequiredDescribeBudgetsRequestRequestTypeDef, _OptionalDescribeBudgetsRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
-    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeNotificationsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
@@ -478,89 +454,83 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeNotificationsForBudgetRequestRequestTypeDef(
     _RequiredDescribeNotificationsForBudgetRequestRequestTypeDef,
     _OptionalDescribeNotificationsForBudgetRequestRequestTypeDef,
 ):
     pass
 
+
 ExecuteBudgetActionRequestRequestTypeDef = TypedDict(
     "ExecuteBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
 
-ExecuteBudgetActionResponseTypeDef = TypedDict(
-    "ExecuteBudgetActionResponseTypeDef",
+_RequiredAutoAdjustDataOutputTypeDef = TypedDict(
+    "_RequiredAutoAdjustDataOutputTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ExecutionType": ExecutionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AutoAdjustType": AutoAdjustTypeType,
     },
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalAutoAdjustDataOutputTypeDef = TypedDict(
+    "_OptionalAutoAdjustDataOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HistoricalOptions": HistoricalOptionsTypeDef,
+        "LastAutoAdjustTime": datetime,
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
 
-DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
-    "DescribeSubscribersForNotificationResponseTypeDef",
-    {
-        "Subscribers": List[SubscriberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class AutoAdjustDataOutputTypeDef(
+    _RequiredAutoAdjustDataOutputTypeDef, _OptionalAutoAdjustDataOutputTypeDef
+):
+    pass
+
 
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
     "_OptionalAutoAdjustDataTypeDef",
     {
         "HistoricalOptions": HistoricalOptionsTypeDef,
-        "LastAutoAdjustTime": Union[datetime, str],
+        "LastAutoAdjustTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class AutoAdjustDataTypeDef(_RequiredAutoAdjustDataTypeDef, _OptionalAutoAdjustDataTypeDef):
     pass
 
+
+TimePeriodTypeDef = TypedDict(
+    "TimePeriodTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+    },
+    total=False,
+)
+
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
         "Notifications": List[NotificationTypeDef],
         "BudgetName": str,
     },
     total=False,
@@ -601,45 +571,14 @@
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "Subscriber": SubscriberTypeDef,
     },
 )
 
-DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    {
-        "Notifications": List[NotificationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
     },
@@ -649,20 +588,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeSubscribersForNotificationRequestRequestTypeDef(
     _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef,
     _OptionalDescribeSubscribersForNotificationRequestRequestTypeDef,
 ):
     pass
 
+
 NotificationWithSubscribersTypeDef = TypedDict(
     "NotificationWithSubscribersTypeDef",
     {
         "Notification": NotificationTypeDef,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
@@ -698,27 +639,224 @@
     "_OptionalCalculatedSpendTypeDef",
     {
         "ForecastedSpend": SpendTypeDef,
     },
     total=False,
 )
 
+
 class CalculatedSpendTypeDef(_RequiredCalculatedSpendTypeDef, _OptionalCalculatedSpendTypeDef):
     pass
 
+
 BudgetedAndActualAmountsTypeDef = TypedDict(
     "BudgetedAndActualAmountsTypeDef",
     {
         "BudgetedAmount": SpendTypeDef,
         "ActualAmount": SpendTypeDef,
-        "TimePeriod": TimePeriodTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
+    },
+    total=False,
+)
+
+CreateBudgetActionResponseTypeDef = TypedDict(
+    "CreateBudgetActionResponseTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    {
+        "Notifications": List[NotificationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
+    "DescribeSubscribersForNotificationResponseTypeDef",
+    {
+        "Subscribers": List[SubscriberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExecuteBudgetActionResponseTypeDef = TypedDict(
+    "ExecuteBudgetActionResponseTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ExecutionType": ExecutionTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DefinitionOutputTypeDef = TypedDict(
+    "DefinitionOutputTypeDef",
+    {
+        "IamActionDefinition": IamActionDefinitionOutputTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionOutputTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
+DefinitionTypeDef = TypedDict(
+    "DefinitionTypeDef",
+    {
+        "IamActionDefinition": IamActionDefinitionTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
+    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
+    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -726,26 +864,28 @@
     )
 )
 _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "TimePeriod": TimePeriodTypeDef,
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
+
 class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
     _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -756,42 +896,46 @@
         "TimePeriod": TimePeriodTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeBudgetActionHistoriesRequestRequestTypeDef(
     _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
     _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "TimePeriod": TimePeriodTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -801,39 +945,60 @@
         "TimePeriod": TimePeriodTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
-DefinitionTypeDef = TypedDict(
-    "DefinitionTypeDef",
-    {
-        "IamActionDefinition": IamActionDefinitionTypeDef,
-        "ScpActionDefinition": ScpActionDefinitionTypeDef,
-        "SsmActionDefinition": SsmActionDefinitionTypeDef,
-    },
-    total=False,
-)
 
+TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodOutputTypeDef]
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBudgetOutputTypeDef = TypedDict(
+    "_RequiredBudgetOutputTypeDef",
+    {
+        "BudgetName": str,
+        "TimeUnit": TimeUnitType,
+        "BudgetType": BudgetTypeType,
+    },
+)
+_OptionalBudgetOutputTypeDef = TypedDict(
+    "_OptionalBudgetOutputTypeDef",
+    {
+        "BudgetLimit": SpendTypeDef,
+        "PlannedBudgetLimits": Dict[str, SpendTypeDef],
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
+        "CalculatedSpend": CalculatedSpendTypeDef,
+        "LastUpdatedTime": datetime,
+        "AutoAdjustData": AutoAdjustDataOutputTypeDef,
     },
+    total=False,
 )
 
+
+class BudgetOutputTypeDef(_RequiredBudgetOutputTypeDef, _OptionalBudgetOutputTypeDef):
+    pass
+
+
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
     },
@@ -843,23 +1008,25 @@
     {
         "BudgetLimit": SpendTypeDef,
         "PlannedBudgetLimits": Mapping[str, SpendTypeDef],
         "CostFilters": Mapping[str, Sequence[str]],
         "CostTypes": CostTypesTypeDef,
         "TimePeriod": TimePeriodTypeDef,
         "CalculatedSpend": CalculatedSpendTypeDef,
-        "LastUpdatedTime": Union[datetime, str],
+        "LastUpdatedTime": TimestampTypeDef,
         "AutoAdjustData": AutoAdjustDataTypeDef,
     },
     total=False,
 )
 
+
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
 
+
 BudgetPerformanceHistoryTypeDef = TypedDict(
     "BudgetPerformanceHistoryTypeDef",
     {
         "BudgetName": str,
         "BudgetType": BudgetTypeType,
         "CostFilters": Dict[str, List[str]],
         "CostTypes": CostTypesTypeDef,
@@ -873,15 +1040,15 @@
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionTypeDef,
+        "Definition": DefinitionOutputTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
         "Subscribers": List[SubscriberTypeDef],
     },
 )
 
@@ -896,14 +1063,15 @@
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
 
+DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionOutputTypeDef]
 _RequiredUpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -917,20 +1085,40 @@
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
     total=False,
 )
 
+
 class UpdateBudgetActionRequestRequestTypeDef(
     _RequiredUpdateBudgetActionRequestRequestTypeDef,
     _OptionalUpdateBudgetActionRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
+    {
+        "Budget": BudgetOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
+    {
+        "Budgets": List[BudgetOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetOutputTypeDef]
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
@@ -938,50 +1126,35 @@
     "_OptionalCreateBudgetRequestRequestTypeDef",
     {
         "NotificationsWithSubscribers": Sequence[NotificationWithSubscribersTypeDef],
     },
     total=False,
 )
 
+
 class CreateBudgetRequestRequestTypeDef(
     _RequiredCreateBudgetRequestRequestTypeDef, _OptionalCreateBudgetRequestRequestTypeDef
 ):
     pass
 
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
-    {
-        "Budgets": List[BudgetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "NewBudget": BudgetTypeDef,
     },
 )
 
 DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     {
         "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
@@ -991,54 +1164,54 @@
 
 DeleteBudgetActionResponseTypeDef = TypedDict(
     "DeleteBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBudgetActionResponseTypeDef = TypedDict(
     "DescribeBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBudgetActionsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForAccountResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBudgetActionsForBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBudgetActionResponseTypeDef = TypedDict(
     "UpdateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
@@ -1049,10 +1222,10 @@
 )
 
 DescribeBudgetActionHistoriesResponseTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesResponseTypeDef",
     {
         "ActionHistories": List[ActionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/PKG-INFO` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore budgets type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore budgets type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-budgets"></a>
 
 # types-aiobotocore-budgets
 
 [![PyPI - types-aiobotocore-budgets](https://img.shields.io/pypi/v/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-budgets?color=blue)](https://pypistats.org/packages/types-aiobotocore-budgets)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [types-aiobotocore-budgets docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/).
 
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
@@ -354,95 +353,106 @@
 )
 
 
 def check_value(value: ActionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_budgets.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_budgets.type_defs import (
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
+    TimestampTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
-    TimePeriodTypeDef,
-    CreateBudgetActionResponseTypeDef,
+    TimePeriodOutputTypeDef,
+    ResponseMetadataTypeDef,
+    IamActionDefinitionOutputTypeDef,
+    ScpActionDefinitionOutputTypeDef,
+    SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
-    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestRequestTypeDef,
-    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestRequestTypeDef,
-    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
-    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
-    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
-    ExecuteBudgetActionResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeSubscribersForNotificationResponseTypeDef,
+    AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
+    TimePeriodTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
-    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
+    CreateBudgetActionResponseTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    DescribeSubscribersForNotificationResponseTypeDef,
+    ExecuteBudgetActionResponseTypeDef,
+    DefinitionOutputTypeDef,
+    DefinitionTypeDef,
+    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    DefinitionTypeDef,
+    TimePeriodUnionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
+    BudgetOutputTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
+    DefinitionUnionTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
-    CreateBudgetRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
+    BudgetUnionTypeDef,
+    CreateBudgetRequestRequestTypeDef,
     UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_value() -> ActionThresholdTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/SOURCES.txt` & `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*


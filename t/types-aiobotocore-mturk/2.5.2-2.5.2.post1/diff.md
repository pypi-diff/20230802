# Comparing `tmp/types-aiobotocore-mturk-2.5.2.tar.gz` & `tmp/types-aiobotocore-mturk-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mturk-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-mturk-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:42 2023, max compression
```

## Comparing `types-aiobotocore-mturk-2.5.2.tar` & `types-aiobotocore-mturk-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.298595 types-aiobotocore-mturk-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-08 01:44:02.298595 types-aiobotocore-mturk-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.298595 types-aiobotocore-mturk-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:35:32.000000 types-aiobotocore-mturk-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.298595 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35331 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37596 2023-07-08 01:35:35.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37541 2023-07-08 01:35:35.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:34.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.298595 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-08 01:44:02.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-08 01:44:02.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:44:02.000000 types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.929513 types-aiobotocore-mturk-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18798 2023-08-02 14:52:42.921513 types-aiobotocore-mturk-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:42.929513 types-aiobotocore-mturk-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:43:49.000000 types-aiobotocore-mturk-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.921513 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35409 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35352 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39546 2023-08-02 14:43:51.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39487 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.921513 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18798 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mturk-2.5.2/LICENSE` & `types-aiobotocore-mturk-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2/PKG-INFO` & `types-aiobotocore-mturk-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mturk
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MTurk 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MTurk 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore mturk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore mturk type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mturk"></a>
 
 # types-aiobotocore-mturk
 
 [![PyPI - types-aiobotocore-mturk](https://img.shields.io/pypi/v/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mturk?color=blue)](https://pypistats.org/packages/types-aiobotocore-mturk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mturk)](https://pepy.tech/project/types-aiobotocore-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MTurk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [types-aiobotocore-mturk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/).
 
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
@@ -358,116 +357,123 @@
 )
 
 
 def check_value(value: AssignmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mturk.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mturk.type_defs import (
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    CreateHITTypeResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
-    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
-    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
-    UpdateExpirationForHITRequestRequestTypeDef,
+    TimestampTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
+    CreateHITTypeResponseTypeDef,
+    GetAccountBalanceResponseTypeDef,
+    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationRequirementTypeDef,
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
+    PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
+    UpdateExpirationForHITRequestRequestTypeDef,
     HITTypeDef,
+    QualificationRequirementUnionTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
+    ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
-    ListReviewPolicyResultsForHITResponseTypeDef,
+    ReviewPolicyUnionTypeDef,
 )
 
 
-def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
+def get_value() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mturk-2.5.2/README.md` & `types-aiobotocore-mturk-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-mturk"></a>
 
 # types-aiobotocore-mturk
 
 [![PyPI - types-aiobotocore-mturk](https://img.shields.io/pypi/v/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mturk?color=blue)](https://pypistats.org/packages/types-aiobotocore-mturk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mturk)](https://pepy.tech/project/types-aiobotocore-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MTurk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [types-aiobotocore-mturk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/).
 
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
@@ -325,116 +325,123 @@
 )
 
 
 def check_value(value: AssignmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mturk.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mturk.type_defs import (
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    CreateHITTypeResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
-    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
-    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
-    UpdateExpirationForHITRequestRequestTypeDef,
+    TimestampTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
+    CreateHITTypeResponseTypeDef,
+    GetAccountBalanceResponseTypeDef,
+    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationRequirementTypeDef,
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
+    PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
+    UpdateExpirationForHITRequestRequestTypeDef,
     HITTypeDef,
+    QualificationRequirementUnionTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
+    ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
-    ListReviewPolicyResultsForHITResponseTypeDef,
+    ReviewPolicyUnionTypeDef,
 )
 
 
-def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
+def get_value() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mturk-2.5.2/setup.py` & `types-aiobotocore-mturk-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mturk",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MTurk 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore mturk type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore mturk type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mturk": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/"
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/__init__.py` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/__init__.pyi` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/__main__.py` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MTurk 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.MTurk 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/client.py` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("mturk") as client:
         client: MTurkClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AssignmentStatusType,
     EventTypeType,
@@ -60,16 +59,17 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
-    QualificationRequirementTypeDef,
-    ReviewPolicyTypeDef,
+    QualificationRequirementUnionTypeDef,
+    ReviewPolicyUnionTypeDef,
+    TimestampTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -182,18 +182,18 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -205,15 +205,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit_type)
         """
@@ -223,16 +223,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
 
@@ -580,15 +580,15 @@
         notification specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.send_test_event_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#send_test_event_notification)
         """
 
     async def update_expiration_for_hit(
-        self, *, HITId: str, ExpireAt: Union[datetime, str]
+        self, *, HITId: str, ExpireAt: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         The `UpdateExpirationForHIT` operation allows you update the expiration time of
         a HIT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_expiration_for_hit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#update_expiration_for_hit)
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/client.pyi` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("mturk") as client:
         client: MTurkClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AssignmentStatusType,
     EventTypeType,
@@ -60,16 +59,17 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
-    QualificationRequirementTypeDef,
-    ReviewPolicyTypeDef,
+    QualificationRequirementUnionTypeDef,
+    ReviewPolicyUnionTypeDef,
+    TimestampTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,18 +171,18 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -193,15 +193,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit_type)
         """
@@ -210,16 +210,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
 
@@ -538,15 +538,15 @@
         a notification message as if a HIT event occurred, according to the provided
         notification specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.send_test_event_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#send_test_event_notification)
         """
     async def update_expiration_for_hit(
-        self, *, HITId: str, ExpireAt: Union[datetime, str]
+        self, *, HITId: str, ExpireAt: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         The `UpdateExpirationForHIT` operation allows you update the expiration time of
         a HIT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_expiration_for_hit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#update_expiration_for_hit)
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/literals.py` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/literals.pyi` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/paginator.py` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
 
@@ -104,60 +104,60 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listbonuspaymentspaginator)
         """
 
 
 class ListHITsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitspaginator)
         """
 
 
 class ListHITsForQualificationTypePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitsforqualificationtypepaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHITsForQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitsforqualificationtypepaginator)
         """
 
 
 class ListQualificationRequestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationrequestspaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQualificationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationrequestspaginator)
         """
 
 
@@ -169,15 +169,15 @@
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationtypespaginator)
         """
 
 
@@ -188,30 +188,30 @@
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReviewableHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listreviewablehitspaginator)
         """
 
 
 class ListWorkerBlocksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerblockspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkerBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerblockspaginator)
         """
 
 
@@ -222,13 +222,13 @@
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/paginator.pyi` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
 class ListBonusPaymentsPaginator(AioPaginator):
@@ -100,57 +100,57 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listbonuspaymentspaginator)
         """
 
 class ListHITsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitspaginator)
         """
 
 class ListHITsForQualificationTypePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitsforqualificationtypepaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHITsForQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listhitsforqualificationtypepaginator)
         """
 
 class ListQualificationRequestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationrequestspaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQualificationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationrequestspaginator)
         """
 
 class ListQualificationTypesPaginator(AioPaginator):
@@ -161,15 +161,15 @@
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationtypespaginator)
         """
 
 class ListReviewableHITsPaginator(AioPaginator):
@@ -179,29 +179,29 @@
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReviewableHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listreviewablehitspaginator)
         """
 
 class ListWorkerBlocksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerblockspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkerBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerblockspaginator)
         """
 
 class ListWorkersWithQualificationTypePaginator(AioPaginator):
@@ -211,13 +211,13 @@
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/type_defs.py` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_mturk.type_defs import AcceptQualificationRequestRequestRequestTypeDef
 
-    data: AcceptQualificationRequestRequestRequestTypeDef = {...}
+    data: AcceptQualificationRequestRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -41,96 +41,103 @@
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
     "HITLayoutParameterTypeDef",
-    "CreateHITTypeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateQualificationTypeRequestRequestTypeDef",
     "QualificationTypeTypeDef",
     "CreateWorkerBlockRequestRequestTypeDef",
     "DeleteHITRequestRequestTypeDef",
     "DeleteQualificationTypeRequestRequestTypeDef",
     "DeleteWorkerBlockRequestRequestTypeDef",
     "DisassociateQualificationFromWorkerRequestRequestTypeDef",
-    "GetAccountBalanceResponseTypeDef",
     "GetAssignmentRequestRequestTypeDef",
     "GetFileUploadURLRequestRequestTypeDef",
-    "GetFileUploadURLResponseTypeDef",
     "GetHITRequestRequestTypeDef",
     "GetQualificationScoreRequestRequestTypeDef",
     "GetQualificationTypeRequestRequestTypeDef",
-    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssignmentsForHITRequestRequestTypeDef",
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
     "ListBonusPaymentsRequestRequestTypeDef",
-    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
     "ListHITsForQualificationTypeRequestRequestTypeDef",
-    "ListHITsRequestListHITsPaginateTypeDef",
     "ListHITsRequestRequestTypeDef",
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationRequestsRequestRequestTypeDef",
     "QualificationRequestTypeDef",
-    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListQualificationTypesRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITRequestRequestTypeDef",
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
-    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
-    "UpdateExpirationForHITRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
+    "CreateHITTypeResponseTypeDef",
+    "GetAccountBalanceResponseTypeDef",
+    "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
+    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    "ListHITsRequestListHITsPaginateTypeDef",
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
+    "QualificationRequirementOutputTypeDef",
     "QualificationRequirementTypeDef",
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
+    "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
+    "UpdateExpirationForHITRequestRequestTypeDef",
     "HITTypeDef",
+    "QualificationRequirementUnionTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
+    "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
+    "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
-    "ListReviewPolicyResultsForHITResponseTypeDef",
+    "ReviewPolicyUnionTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -255,19 +262,22 @@
     "HITLayoutParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CreateHITTypeResponseTypeDef = TypedDict(
-    "CreateHITTypeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "HITTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQualificationTypeRequestRequestTypeDef",
     {
         "Name": str,
@@ -379,23 +389,14 @@
 class DisassociateQualificationFromWorkerRequestRequestTypeDef(
     _RequiredDisassociateQualificationFromWorkerRequestRequestTypeDef,
     _OptionalDisassociateQualificationFromWorkerRequestRequestTypeDef,
 ):
     pass
 
 
-GetAccountBalanceResponseTypeDef = TypedDict(
-    "GetAccountBalanceResponseTypeDef",
-    {
-        "AvailableBalance": str,
-        "OnHoldBalance": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssignmentRequestRequestTypeDef = TypedDict(
     "GetAssignmentRequestRequestTypeDef",
     {
         "AssignmentId": str,
     },
 )
 
@@ -403,22 +404,14 @@
     "GetFileUploadURLRequestRequestTypeDef",
     {
         "AssignmentId": str,
         "QuestionIdentifier": str,
     },
 )
 
-GetFileUploadURLResponseTypeDef = TypedDict(
-    "GetFileUploadURLResponseTypeDef",
-    {
-        "FileUploadURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHITRequestRequestTypeDef = TypedDict(
     "GetHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 
@@ -433,37 +426,24 @@
 GetQualificationTypeRequestRequestTypeDef = TypedDict(
     "GetQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 
-_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "HITId": str,
-    },
-)
-_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AssignmentStatuses": Sequence[AssignmentStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
-    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssignmentsForHITRequestRequestTypeDef = TypedDict(
     "_RequiredListAssignmentsForHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalListAssignmentsForHITRequestRequestTypeDef = TypedDict(
@@ -480,57 +460,25 @@
 class ListAssignmentsForHITRequestRequestTypeDef(
     _RequiredListAssignmentsForHITRequestRequestTypeDef,
     _OptionalListAssignmentsForHITRequestRequestTypeDef,
 ):
     pass
 
 
-ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    {
-        "HITId": str,
-        "AssignmentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBonusPaymentsRequestRequestTypeDef = TypedDict(
     "ListBonusPaymentsRequestRequestTypeDef",
     {
         "HITId": str,
         "AssignmentId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
-    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListHITsForQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -546,40 +494,23 @@
 class ListHITsForQualificationTypeRequestRequestTypeDef(
     _RequiredListHITsForQualificationTypeRequestRequestTypeDef,
     _OptionalListHITsForQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
-ListHITsRequestListHITsPaginateTypeDef = TypedDict(
-    "ListHITsRequestListHITsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHITsRequestRequestTypeDef = TypedDict(
     "ListHITsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQualificationRequestsRequestRequestTypeDef = TypedDict(
     "ListQualificationRequestsRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -595,38 +526,14 @@
         "Test": str,
         "Answer": str,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
-_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "MustBeRequestable": bool,
-    },
-)
-_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "Query": str,
-        "MustBeOwnedByCaller": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
-    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListQualificationTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListQualificationTypesRequestRequestTypeDef",
     {
         "MustBeRequestable": bool,
     },
 )
 _OptionalListQualificationTypesRequestRequestTypeDef = TypedDict(
@@ -670,43 +577,25 @@
 class ListReviewPolicyResultsForHITRequestRequestTypeDef(
     _RequiredListReviewPolicyResultsForHITRequestRequestTypeDef,
     _OptionalListReviewPolicyResultsForHITRequestRequestTypeDef,
 ):
     pass
 
 
-ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    {
-        "HITTypeId": str,
-        "Status": ReviewableHITStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReviewableHITsRequestRequestTypeDef = TypedDict(
     "ListReviewableHITsRequestRequestTypeDef",
     {
         "HITTypeId": str,
         "Status": ReviewableHITStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkerBlocksRequestRequestTypeDef = TypedDict(
     "ListWorkerBlocksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -717,37 +606,14 @@
     {
         "WorkerId": str,
         "Reason": str,
     },
     total=False,
 )
 
-_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "Status": QualificationStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
-    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersWithQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -812,20 +678,19 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ParameterMapEntryOutputTypeDef = TypedDict(
+    "ParameterMapEntryOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Values": List[str],
     },
     total=False,
 )
 
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
@@ -861,25 +726,14 @@
 class RejectQualificationRequestRequestRequestTypeDef(
     _RequiredRejectQualificationRequestRequestRequestTypeDef,
     _OptionalRejectQualificationRequestRequestRequestTypeDef,
 ):
     pass
 
 
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
 ReviewActionDetailTypeDef = TypedDict(
     "ReviewActionDetailTypeDef",
     {
         "ActionId": str,
         "ActionName": str,
         "TargetId": str,
         "TargetType": str,
@@ -924,22 +778,15 @@
 
 class SendBonusRequestRequestTypeDef(
     _RequiredSendBonusRequestRequestTypeDef, _OptionalSendBonusRequestRequestTypeDef
 ):
     pass
 
 
-UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
-    "UpdateExpirationForHITRequestRequestTypeDef",
-    {
-        "HITId": str,
-        "ExpireAt": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHITReviewStatusRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
@@ -991,88 +838,275 @@
 class UpdateQualificationTypeRequestRequestTypeDef(
     _RequiredUpdateQualificationTypeRequestRequestTypeDef,
     _OptionalUpdateQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
+CreateHITTypeResponseTypeDef = TypedDict(
+    "CreateHITTypeResponseTypeDef",
+    {
+        "HITTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountBalanceResponseTypeDef = TypedDict(
+    "GetAccountBalanceResponseTypeDef",
+    {
+        "AvailableBalance": str,
+        "OnHoldBalance": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFileUploadURLResponseTypeDef = TypedDict(
+    "GetFileUploadURLResponseTypeDef",
+    {
+        "FileUploadURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAssignmentsForHITResponseTypeDef = TypedDict(
     "ListAssignmentsForHITResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Assignments": List[AssignmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBonusPaymentsResponseTypeDef = TypedDict(
     "ListBonusPaymentsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "BonusPayments": List[BonusPaymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQualificationTypeResponseTypeDef = TypedDict(
     "CreateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQualificationTypeResponseTypeDef = TypedDict(
     "GetQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQualificationTypesResponseTypeDef = TypedDict(
     "ListQualificationTypesResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationTypes": List[QualificationTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQualificationTypeResponseTypeDef = TypedDict(
     "UpdateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "HITId": str,
+    },
+)
+_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "AssignmentStatuses": Sequence[AssignmentStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
+    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+):
+    pass
+
+
+ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    {
+        "HITId": str,
+        "AssignmentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
+    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+):
+    pass
+
+
+ListHITsRequestListHITsPaginateTypeDef = TypedDict(
+    "ListHITsRequestListHITsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "MustBeRequestable": bool,
+    },
+)
+_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "Query": str,
+        "MustBeOwnedByCaller": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
+    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+):
+    pass
+
+
+ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    {
+        "HITTypeId": str,
+        "Status": ReviewableHITStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "Status": QualificationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
+    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+):
+    pass
+
+
 ListQualificationRequestsResponseTypeDef = TypedDict(
     "ListQualificationRequestsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationRequests": List[QualificationRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkerBlocksResponseTypeDef = TypedDict(
     "ListWorkerBlocksResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredQualificationRequirementOutputTypeDef = TypedDict(
+    "_RequiredQualificationRequirementOutputTypeDef",
+    {
+        "QualificationTypeId": str,
+        "Comparator": ComparatorType,
+    },
+)
+_OptionalQualificationRequirementOutputTypeDef = TypedDict(
+    "_OptionalQualificationRequirementOutputTypeDef",
+    {
+        "IntegerValues": List[int],
+        "LocaleValues": List[LocaleTypeDef],
+        "RequiredToPreview": bool,
+        "ActionsGuarded": HITAccessActionsType,
     },
+    total=False,
 )
 
+
+class QualificationRequirementOutputTypeDef(
+    _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
+):
+    pass
+
+
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
@@ -1138,18 +1172,28 @@
     pass
 
 
 NotifyWorkersResponseTypeDef = TypedDict(
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PolicyParameterOutputTypeDef = TypedDict(
+    "PolicyParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MapEntries": List[ParameterMapEntryOutputTypeDef],
+    },
+    total=False,
+)
+
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MapEntries": Sequence[ParameterMapEntryTypeDef],
     },
@@ -1161,40 +1205,22 @@
     {
         "ReviewResults": List[ReviewResultDetailTypeDef],
         "ReviewActions": List[ReviewActionDetailTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
+UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
+    "UpdateExpirationForHITRequestRequestTypeDef",
     {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "HITId": str,
+        "ExpireAt": TimestampTypeDef,
     },
-    total=False,
 )
 
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
-
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1206,41 +1232,65 @@
         "HITStatus": HITStatusType,
         "MaxAssignments": int,
         "Reward": str,
         "AutoApprovalDelayInSeconds": int,
         "Expiration": datetime,
         "AssignmentDurationInSeconds": int,
         "RequesterAnnotation": str,
-        "QualificationRequirements": List[QualificationRequirementTypeDef],
+        "QualificationRequirements": List[QualificationRequirementOutputTypeDef],
         "HITReviewStatus": HITReviewStatusType,
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
+QualificationRequirementUnionTypeDef = Union[
+    QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef
+]
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
     "ListWorkersWithQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredReviewPolicyOutputTypeDef = TypedDict(
+    "_RequiredReviewPolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+    },
+)
+_OptionalReviewPolicyOutputTypeDef = TypedDict(
+    "_OptionalReviewPolicyOutputTypeDef",
+    {
+        "Parameters": List[PolicyParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ReviewPolicyOutputTypeDef(
+    _RequiredReviewPolicyOutputTypeDef, _OptionalReviewPolicyOutputTypeDef
+):
+    pass
+
+
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyTypeDef = TypedDict(
@@ -1256,70 +1306,109 @@
     pass
 
 
 CreateHITResponseTypeDef = TypedDict(
     "CreateHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHITWithHITTypeResponseTypeDef = TypedDict(
     "CreateHITWithHITTypeResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssignmentResponseTypeDef = TypedDict(
     "GetAssignmentResponseTypeDef",
     {
         "Assignment": AssignmentTypeDef,
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHITResponseTypeDef = TypedDict(
     "GetHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsForQualificationTypeResponseTypeDef = TypedDict(
     "ListHITsForQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsResponseTypeDef = TypedDict(
     "ListHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReviewableHITsResponseTypeDef = TypedDict(
     "ListReviewableHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
+
+ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
+    "ListReviewPolicyResultsForHITResponseTypeDef",
+    {
+        "HITId": str,
+        "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
+        "HITReviewPolicy": ReviewPolicyOutputTypeDef,
+        "AssignmentReviewReport": ReviewReportTypeDef,
+        "HITReviewReport": ReviewReportTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
@@ -1333,15 +1422,15 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
@@ -1380,19 +1469,8 @@
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
 
 
-ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
-    "ListReviewPolicyResultsForHITResponseTypeDef",
-    {
-        "HITId": str,
-        "AssignmentReviewPolicy": ReviewPolicyTypeDef,
-        "HITReviewPolicy": ReviewPolicyTypeDef,
-        "AssignmentReviewReport": ReviewReportTypeDef,
-        "HITReviewReport": ReviewReportTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+ReviewPolicyUnionTypeDef = Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef]
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk/type_defs.pyi` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_mturk.type_defs import AcceptQualificationRequestRequestRequestTypeDef
 
-    data: AcceptQualificationRequestRequestRequestTypeDef = {...}
+    data: AcceptQualificationRequestRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -40,96 +40,103 @@
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
     "HITLayoutParameterTypeDef",
-    "CreateHITTypeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateQualificationTypeRequestRequestTypeDef",
     "QualificationTypeTypeDef",
     "CreateWorkerBlockRequestRequestTypeDef",
     "DeleteHITRequestRequestTypeDef",
     "DeleteQualificationTypeRequestRequestTypeDef",
     "DeleteWorkerBlockRequestRequestTypeDef",
     "DisassociateQualificationFromWorkerRequestRequestTypeDef",
-    "GetAccountBalanceResponseTypeDef",
     "GetAssignmentRequestRequestTypeDef",
     "GetFileUploadURLRequestRequestTypeDef",
-    "GetFileUploadURLResponseTypeDef",
     "GetHITRequestRequestTypeDef",
     "GetQualificationScoreRequestRequestTypeDef",
     "GetQualificationTypeRequestRequestTypeDef",
-    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssignmentsForHITRequestRequestTypeDef",
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
     "ListBonusPaymentsRequestRequestTypeDef",
-    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
     "ListHITsForQualificationTypeRequestRequestTypeDef",
-    "ListHITsRequestListHITsPaginateTypeDef",
     "ListHITsRequestRequestTypeDef",
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationRequestsRequestRequestTypeDef",
     "QualificationRequestTypeDef",
-    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListQualificationTypesRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITRequestRequestTypeDef",
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
-    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
-    "UpdateExpirationForHITRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
+    "CreateHITTypeResponseTypeDef",
+    "GetAccountBalanceResponseTypeDef",
+    "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
+    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    "ListHITsRequestListHITsPaginateTypeDef",
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
+    "QualificationRequirementOutputTypeDef",
     "QualificationRequirementTypeDef",
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
+    "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
+    "UpdateExpirationForHITRequestRequestTypeDef",
     "HITTypeDef",
+    "QualificationRequirementUnionTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
+    "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
+    "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
-    "ListReviewPolicyResultsForHITResponseTypeDef",
+    "ReviewPolicyUnionTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -246,19 +253,22 @@
     "HITLayoutParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CreateHITTypeResponseTypeDef = TypedDict(
-    "CreateHITTypeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "HITTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQualificationTypeRequestRequestTypeDef",
     {
         "Name": str,
@@ -364,23 +374,14 @@
 
 class DisassociateQualificationFromWorkerRequestRequestTypeDef(
     _RequiredDisassociateQualificationFromWorkerRequestRequestTypeDef,
     _OptionalDisassociateQualificationFromWorkerRequestRequestTypeDef,
 ):
     pass
 
-GetAccountBalanceResponseTypeDef = TypedDict(
-    "GetAccountBalanceResponseTypeDef",
-    {
-        "AvailableBalance": str,
-        "OnHoldBalance": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssignmentRequestRequestTypeDef = TypedDict(
     "GetAssignmentRequestRequestTypeDef",
     {
         "AssignmentId": str,
     },
 )
 
@@ -388,22 +389,14 @@
     "GetFileUploadURLRequestRequestTypeDef",
     {
         "AssignmentId": str,
         "QuestionIdentifier": str,
     },
 )
 
-GetFileUploadURLResponseTypeDef = TypedDict(
-    "GetFileUploadURLResponseTypeDef",
-    {
-        "FileUploadURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHITRequestRequestTypeDef = TypedDict(
     "GetHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 
@@ -418,35 +411,24 @@
 GetQualificationTypeRequestRequestTypeDef = TypedDict(
     "GetQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 
-_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "HITId": str,
-    },
-)
-_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AssignmentStatuses": Sequence[AssignmentStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
-    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssignmentsForHITRequestRequestTypeDef = TypedDict(
     "_RequiredListAssignmentsForHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalListAssignmentsForHITRequestRequestTypeDef = TypedDict(
@@ -461,55 +443,25 @@
 
 class ListAssignmentsForHITRequestRequestTypeDef(
     _RequiredListAssignmentsForHITRequestRequestTypeDef,
     _OptionalListAssignmentsForHITRequestRequestTypeDef,
 ):
     pass
 
-ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    {
-        "HITId": str,
-        "AssignmentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBonusPaymentsRequestRequestTypeDef = TypedDict(
     "ListBonusPaymentsRequestRequestTypeDef",
     {
         "HITId": str,
         "AssignmentId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
-    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-):
-    pass
-
 _RequiredListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListHITsForQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -523,40 +475,23 @@
 
 class ListHITsForQualificationTypeRequestRequestTypeDef(
     _RequiredListHITsForQualificationTypeRequestRequestTypeDef,
     _OptionalListHITsForQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
-ListHITsRequestListHITsPaginateTypeDef = TypedDict(
-    "ListHITsRequestListHITsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHITsRequestRequestTypeDef = TypedDict(
     "ListHITsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQualificationRequestsRequestRequestTypeDef = TypedDict(
     "ListQualificationRequestsRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -572,36 +507,14 @@
         "Test": str,
         "Answer": str,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
-_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "MustBeRequestable": bool,
-    },
-)
-_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "Query": str,
-        "MustBeOwnedByCaller": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
-    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListQualificationTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListQualificationTypesRequestRequestTypeDef",
     {
         "MustBeRequestable": bool,
     },
 )
 _OptionalListQualificationTypesRequestRequestTypeDef = TypedDict(
@@ -641,43 +554,25 @@
 
 class ListReviewPolicyResultsForHITRequestRequestTypeDef(
     _RequiredListReviewPolicyResultsForHITRequestRequestTypeDef,
     _OptionalListReviewPolicyResultsForHITRequestRequestTypeDef,
 ):
     pass
 
-ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    {
-        "HITTypeId": str,
-        "Status": ReviewableHITStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReviewableHITsRequestRequestTypeDef = TypedDict(
     "ListReviewableHITsRequestRequestTypeDef",
     {
         "HITTypeId": str,
         "Status": ReviewableHITStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkerBlocksRequestRequestTypeDef = TypedDict(
     "ListWorkerBlocksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -688,35 +583,14 @@
     {
         "WorkerId": str,
         "Reason": str,
     },
     total=False,
 )
 
-_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "Status": QualificationStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
-    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersWithQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -777,20 +651,19 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ParameterMapEntryOutputTypeDef = TypedDict(
+    "ParameterMapEntryOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Values": List[str],
     },
     total=False,
 )
 
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
@@ -824,25 +697,14 @@
 
 class RejectQualificationRequestRequestRequestTypeDef(
     _RequiredRejectQualificationRequestRequestRequestTypeDef,
     _OptionalRejectQualificationRequestRequestRequestTypeDef,
 ):
     pass
 
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
 ReviewActionDetailTypeDef = TypedDict(
     "ReviewActionDetailTypeDef",
     {
         "ActionId": str,
         "ActionName": str,
         "TargetId": str,
         "TargetType": str,
@@ -885,22 +747,15 @@
 )
 
 class SendBonusRequestRequestTypeDef(
     _RequiredSendBonusRequestRequestTypeDef, _OptionalSendBonusRequestRequestTypeDef
 ):
     pass
 
-UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
-    "UpdateExpirationForHITRequestRequestTypeDef",
-    {
-        "HITId": str,
-        "ExpireAt": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHITReviewStatusRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
@@ -948,88 +803,265 @@
 
 class UpdateQualificationTypeRequestRequestTypeDef(
     _RequiredUpdateQualificationTypeRequestRequestTypeDef,
     _OptionalUpdateQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
+CreateHITTypeResponseTypeDef = TypedDict(
+    "CreateHITTypeResponseTypeDef",
+    {
+        "HITTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountBalanceResponseTypeDef = TypedDict(
+    "GetAccountBalanceResponseTypeDef",
+    {
+        "AvailableBalance": str,
+        "OnHoldBalance": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFileUploadURLResponseTypeDef = TypedDict(
+    "GetFileUploadURLResponseTypeDef",
+    {
+        "FileUploadURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAssignmentsForHITResponseTypeDef = TypedDict(
     "ListAssignmentsForHITResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Assignments": List[AssignmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBonusPaymentsResponseTypeDef = TypedDict(
     "ListBonusPaymentsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "BonusPayments": List[BonusPaymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQualificationTypeResponseTypeDef = TypedDict(
     "CreateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQualificationTypeResponseTypeDef = TypedDict(
     "GetQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQualificationTypesResponseTypeDef = TypedDict(
     "ListQualificationTypesResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationTypes": List[QualificationTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQualificationTypeResponseTypeDef = TypedDict(
     "UpdateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "HITId": str,
+    },
+)
+_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "AssignmentStatuses": Sequence[AssignmentStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
+    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+):
+    pass
+
+ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    {
+        "HITId": str,
+        "AssignmentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
+    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+):
+    pass
+
+ListHITsRequestListHITsPaginateTypeDef = TypedDict(
+    "ListHITsRequestListHITsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "MustBeRequestable": bool,
+    },
+)
+_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "Query": str,
+        "MustBeOwnedByCaller": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
+    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+):
+    pass
+
+ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    {
+        "HITTypeId": str,
+        "Status": ReviewableHITStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "Status": QualificationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
+    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+):
+    pass
+
 ListQualificationRequestsResponseTypeDef = TypedDict(
     "ListQualificationRequestsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationRequests": List[QualificationRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkerBlocksResponseTypeDef = TypedDict(
     "ListWorkerBlocksResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredQualificationRequirementOutputTypeDef = TypedDict(
+    "_RequiredQualificationRequirementOutputTypeDef",
+    {
+        "QualificationTypeId": str,
+        "Comparator": ComparatorType,
+    },
+)
+_OptionalQualificationRequirementOutputTypeDef = TypedDict(
+    "_OptionalQualificationRequirementOutputTypeDef",
+    {
+        "IntegerValues": List[int],
+        "LocaleValues": List[LocaleTypeDef],
+        "RequiredToPreview": bool,
+        "ActionsGuarded": HITAccessActionsType,
     },
+    total=False,
 )
 
+class QualificationRequirementOutputTypeDef(
+    _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
+):
+    pass
+
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
@@ -1091,16 +1123,26 @@
 ):
     pass
 
 NotifyWorkersResponseTypeDef = TypedDict(
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PolicyParameterOutputTypeDef = TypedDict(
+    "PolicyParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MapEntries": List[ParameterMapEntryOutputTypeDef],
     },
+    total=False,
 )
 
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -1114,38 +1156,22 @@
     {
         "ReviewResults": List[ReviewResultDetailTypeDef],
         "ReviewActions": List[ReviewActionDetailTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
+UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
+    "UpdateExpirationForHITRequestRequestTypeDef",
     {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "HITId": str,
+        "ExpireAt": TimestampTypeDef,
     },
-    total=False,
 )
 
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1157,41 +1183,63 @@
         "HITStatus": HITStatusType,
         "MaxAssignments": int,
         "Reward": str,
         "AutoApprovalDelayInSeconds": int,
         "Expiration": datetime,
         "AssignmentDurationInSeconds": int,
         "RequesterAnnotation": str,
-        "QualificationRequirements": List[QualificationRequirementTypeDef],
+        "QualificationRequirements": List[QualificationRequirementOutputTypeDef],
         "HITReviewStatus": HITReviewStatusType,
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
+QualificationRequirementUnionTypeDef = Union[
+    QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef
+]
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
     "ListWorkersWithQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredReviewPolicyOutputTypeDef = TypedDict(
+    "_RequiredReviewPolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+    },
+)
+_OptionalReviewPolicyOutputTypeDef = TypedDict(
+    "_OptionalReviewPolicyOutputTypeDef",
+    {
+        "Parameters": List[PolicyParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class ReviewPolicyOutputTypeDef(
+    _RequiredReviewPolicyOutputTypeDef, _OptionalReviewPolicyOutputTypeDef
+):
+    pass
+
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyTypeDef = TypedDict(
@@ -1205,70 +1253,107 @@
 class ReviewPolicyTypeDef(_RequiredReviewPolicyTypeDef, _OptionalReviewPolicyTypeDef):
     pass
 
 CreateHITResponseTypeDef = TypedDict(
     "CreateHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHITWithHITTypeResponseTypeDef = TypedDict(
     "CreateHITWithHITTypeResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssignmentResponseTypeDef = TypedDict(
     "GetAssignmentResponseTypeDef",
     {
         "Assignment": AssignmentTypeDef,
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHITResponseTypeDef = TypedDict(
     "GetHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsForQualificationTypeResponseTypeDef = TypedDict(
     "ListHITsForQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsResponseTypeDef = TypedDict(
     "ListHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReviewableHITsResponseTypeDef = TypedDict(
     "ListReviewableHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
+ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
+    "ListReviewPolicyResultsForHITResponseTypeDef",
+    {
+        "HITId": str,
+        "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
+        "HITReviewPolicy": ReviewPolicyOutputTypeDef,
+        "AssignmentReviewReport": ReviewReportTypeDef,
+        "HITReviewReport": ReviewReportTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
@@ -1282,15 +1367,15 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
@@ -1325,19 +1410,8 @@
 
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
 
-ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
-    "ListReviewPolicyResultsForHITResponseTypeDef",
-    {
-        "HITId": str,
-        "AssignmentReviewPolicy": ReviewPolicyTypeDef,
-        "HITReviewPolicy": ReviewPolicyTypeDef,
-        "AssignmentReviewReport": ReviewReportTypeDef,
-        "HITReviewReport": ReviewReportTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+ReviewPolicyUnionTypeDef = Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef]
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/PKG-INFO` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mturk
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MTurk 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MTurk 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore mturk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore mturk type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mturk"></a>
 
 # types-aiobotocore-mturk
 
 [![PyPI - types-aiobotocore-mturk](https://img.shields.io/pypi/v/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mturk?color=blue)](https://pypistats.org/packages/types-aiobotocore-mturk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mturk)](https://pepy.tech/project/types-aiobotocore-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MTurk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [types-aiobotocore-mturk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/).
 
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
@@ -358,116 +357,123 @@
 )
 
 
 def check_value(value: AssignmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mturk.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mturk.type_defs import (
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    CreateHITTypeResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
-    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
-    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
-    UpdateExpirationForHITRequestRequestTypeDef,
+    TimestampTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
+    CreateHITTypeResponseTypeDef,
+    GetAccountBalanceResponseTypeDef,
+    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationRequirementTypeDef,
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
+    PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
+    UpdateExpirationForHITRequestRequestTypeDef,
     HITTypeDef,
+    QualificationRequirementUnionTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
+    ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
-    ListReviewPolicyResultsForHITResponseTypeDef,
+    ReviewPolicyUnionTypeDef,
 )
 
 
-def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
+def get_value() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mturk-2.5.2/types_aiobotocore_mturk.egg-info/SOURCES.txt` & `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


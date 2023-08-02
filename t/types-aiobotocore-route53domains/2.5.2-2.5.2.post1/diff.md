# Comparing `tmp/types-aiobotocore-route53domains-2.5.2.tar.gz` & `tmp/types-aiobotocore-route53domains-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53domains-2.5.2.tar", last modified: Sat Jul  8 01:44:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53domains-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:55 2023, max compression
```

## Comparing `types-aiobotocore-route53domains-2.5.2.tar` & `types-aiobotocore-route53domains-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.938808 types-aiobotocore-route53domains-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-07-08 01:44:13.938808 types-aiobotocore-route53domains-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:13.938808 types-aiobotocore-route53domains-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:39:33.000000 types-aiobotocore-route53domains-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.934808 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30808 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-08 01:39:35.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27577 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:34.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.938808 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-07-08 01:44:13.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:13.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:13.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:13.000000 types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.005475 types-aiobotocore-route53domains-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-08-02 14:52:55.001475 types-aiobotocore-route53domains-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:55.005475 types-aiobotocore-route53domains-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.997475 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30925 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30878 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-08-02 14:48:10.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28772 2023-08-02 14:48:10.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.001475 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53domains-2.5.2/LICENSE` & `types-aiobotocore-route53domains-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2/PKG-INFO` & `types-aiobotocore-route53domains-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53domains
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53Domains 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53Domains 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53domains type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53domains type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53domains"></a>
 
 # types-aiobotocore-route53domains
 
 [![PyPI - types-aiobotocore-route53domains](https://img.shields.io/pypi/v/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53domains?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53domains)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53domains)](https://pepy.tech/project/types-aiobotocore-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53Domains 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [types-aiobotocore-route53domains docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/).
 
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
@@ -329,112 +328,117 @@
 )
 
 
 def check_value(value: ContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53domains.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
-    NameserverTypeDef,
+    NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    GetOperationDetailResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListOperationsRequestRequestTypeDef,
+    TimestampTypeDef,
     OperationSummaryTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
-    PaginatorConfigTypeDef,
+    NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
-    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
-    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
+    GetOperationDetailResponseTypeDef,
+    RegisterDomainResponseTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    RenewDomainResponseTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListOperationsRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
+    NameserverUnionTypeDef,
     GetDomainDetailResponseTypeDef,
+    ContactDetailUnionTypeDef,
     RegisterDomainRequestRequestTypeDef,
-    TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
+    TransferDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
+def get_value() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53domains-2.5.2/README.md` & `types-aiobotocore-route53domains-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-route53domains"></a>
 
 # types-aiobotocore-route53domains
 
 [![PyPI - types-aiobotocore-route53domains](https://img.shields.io/pypi/v/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53domains?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53domains)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53domains)](https://pepy.tech/project/types-aiobotocore-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53Domains 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [types-aiobotocore-route53domains docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/).
 
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
@@ -296,112 +296,117 @@
 )
 
 
 def check_value(value: ContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53domains.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
-    NameserverTypeDef,
+    NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    GetOperationDetailResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListOperationsRequestRequestTypeDef,
+    TimestampTypeDef,
     OperationSummaryTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
-    PaginatorConfigTypeDef,
+    NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
-    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
-    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
+    GetOperationDetailResponseTypeDef,
+    RegisterDomainResponseTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    RenewDomainResponseTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListOperationsRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
+    NameserverUnionTypeDef,
     GetDomainDetailResponseTypeDef,
+    ContactDetailUnionTypeDef,
     RegisterDomainRequestRequestTypeDef,
-    TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
+    TransferDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
+def get_value() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53domains-2.5.2/setup.py` & `types-aiobotocore-route53domains-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53domains",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53Domains 2.5.2 service generated with"
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
-    keywords="aiobotocore route53domains type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore route53domains type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53domains": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/"
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/__init__.py` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/__init__.pyi` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/__main__.py` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53Domains 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Route53Domains 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
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

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/client.py` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("route53domains") as client:
         client: Route53DomainsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .paginator import (
     ListDomainsPaginator,
@@ -31,15 +30,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
-    ContactDetailTypeDef,
+    ContactDetailUnionTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
@@ -47,22 +46,23 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    NameserverTypeDef,
+    NameserverUnionTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TransferDomainResponseTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
     ViewBillingResponseTypeDef,
 )
@@ -318,15 +318,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_domains)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#list_domains)
         """
 
     async def list_operations(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...
     ) -> ListOperationsResponseTypeDef:
@@ -370,17 +370,17 @@
         """
 
     async def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
@@ -445,19 +445,19 @@
         """
 
     async def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
-        Nameservers: Sequence[NameserverTypeDef] = ...,
+        Nameservers: Sequence[NameserverUnionTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
@@ -478,17 +478,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#transfer_domain_to_another_aws_account)
         """
 
     async def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: ContactDetailTypeDef = ...,
-        RegistrantContact: ContactDetailTypeDef = ...,
-        TechContact: ContactDetailTypeDef = ...,
+        AdminContact: ContactDetailUnionTypeDef = ...,
+        RegistrantContact: ContactDetailUnionTypeDef = ...,
+        TechContact: ContactDetailUnionTypeDef = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact)
@@ -506,15 +506,19 @@
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact_privacy)
         """
 
     async def update_domain_nameservers(
-        self, *, DomainName: str, Nameservers: Sequence[NameserverTypeDef], FIAuthKey: str = ...
+        self,
+        *,
+        DomainName: str,
+        Nameservers: Sequence[NameserverUnionTypeDef],
+        FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_nameservers)
@@ -529,16 +533,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_tags_for_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_tags_for_domain)
         """
 
     async def view_billing(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...
     ) -> ViewBillingResponseTypeDef:
         """
         Returns all the domain-related billing records for the current Amazon Web
         Services account for a specified period See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ViewBilling).
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/client.pyi` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("route53domains") as client:
         client: Route53DomainsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .paginator import (
     ListDomainsPaginator,
@@ -31,15 +30,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
-    ContactDetailTypeDef,
+    ContactDetailUnionTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
@@ -47,22 +46,23 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    NameserverTypeDef,
+    NameserverUnionTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TransferDomainResponseTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
     ViewBillingResponseTypeDef,
 )
@@ -293,15 +293,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_domains)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#list_domains)
         """
     async def list_operations(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...
     ) -> ListOperationsResponseTypeDef:
@@ -341,17 +341,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#push_domain)
         """
     async def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
@@ -410,19 +410,19 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#retrieve_domain_auth_code)
         """
     async def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
-        Nameservers: Sequence[NameserverTypeDef] = ...,
+        Nameservers: Sequence[NameserverUnionTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
@@ -441,17 +441,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain_to_another_aws_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#transfer_domain_to_another_aws_account)
         """
     async def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: ContactDetailTypeDef = ...,
-        RegistrantContact: ContactDetailTypeDef = ...,
-        TechContact: ContactDetailTypeDef = ...,
+        AdminContact: ContactDetailUnionTypeDef = ...,
+        RegistrantContact: ContactDetailUnionTypeDef = ...,
+        TechContact: ContactDetailUnionTypeDef = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact)
@@ -467,15 +467,19 @@
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact_privacy)
         """
     async def update_domain_nameservers(
-        self, *, DomainName: str, Nameservers: Sequence[NameserverTypeDef], FIAuthKey: str = ...
+        self,
+        *,
+        DomainName: str,
+        Nameservers: Sequence[NameserverUnionTypeDef],
+        FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_nameservers)
@@ -488,16 +492,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_tags_for_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_tags_for_domain)
         """
     async def view_billing(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...
     ) -> ViewBillingResponseTypeDef:
         """
         Returns all the domain-related billing records for the current Amazon Web
         Services account for a specified period See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ViewBilling).
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/literals.py` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/literals.pyi` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/paginator.py` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,121 +23,114 @@
         list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
         list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
         list_prices_paginator: ListPricesPaginator = client.get_paginator("list_prices")
         view_billing_paginator: ViewBillingPaginator = client.get_paginator("view_billing")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .type_defs import (
     FilterConditionTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
+    TimestampTypeDef,
     ViewBillingResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDomainsPaginator",
     "ListOperationsPaginator",
     "ListPricesPaginator",
     "ViewBillingPaginator",
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
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listdomainspaginator)
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listdomainspaginator)
         """
 
-
 class ListOperationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listoperationspaginator)
         """
 
-
 class ListPricesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listpricespaginator)
     """
 
     def paginate(
-        self, *, Tld: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Tld: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listpricespaginator)
         """
 
-
 class ViewBillingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#viewbillingpaginator)
     """
 
     def paginate(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/paginator.pyi` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,114 +23,121 @@
         list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
         list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
         list_prices_paginator: ListPricesPaginator = client.get_paginator("list_prices")
         view_billing_paginator: ViewBillingPaginator = client.get_paginator("view_billing")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .type_defs import (
     FilterConditionTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
+    TimestampTypeDef,
     ViewBillingResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListDomainsPaginator",
     "ListOperationsPaginator",
     "ListPricesPaginator",
     "ViewBillingPaginator",
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
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listdomainspaginator)
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listdomainspaginator)
         """
 
+
 class ListOperationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listoperationspaginator)
         """
 
+
 class ListPricesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listpricespaginator)
     """
 
     def paginate(
-        self, *, Tld: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Tld: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listpricespaginator)
         """
 
+
 class ViewBillingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#viewbillingpaginator)
     """
 
     def paginate(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/type_defs.py` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef
 
-    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = {...}
+    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,137 +35,136 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DnssecSigningAttributesTypeDef",
-    "AssociateDelegationSignerToDomainResponseTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
-    "CheckDomainAvailabilityResponseTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
-    "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     "DnssecKeyTypeDef",
     "PriceWithCurrencyTypeDef",
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
-    "EnableDomainTransferLockResponseTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
-    "GetContactReachabilityStatusResponseTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
-    "NameserverTypeDef",
+    "NameserverOutputTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
-    "GetOperationDetailResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    "ListOperationsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "OperationSummaryTypeDef",
-    "ListPricesRequestListPricesPaginateTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
-    "PaginatorConfigTypeDef",
+    "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
-    "RegisterDomainResponseTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "RenewDomainRequestRequestTypeDef",
-    "RenewDomainResponseTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
-    "ResendContactReachabilityEmailResponseTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+    "UpdateDomainContactPrivacyRequestRequestTypeDef",
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "AssociateDelegationSignerToDomainResponseTypeDef",
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+    "CheckDomainAvailabilityResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DisableDomainTransferLockResponseTypeDef",
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDomainTransferLockResponseTypeDef",
+    "GetContactReachabilityStatusResponseTypeDef",
+    "GetOperationDetailResponseTypeDef",
+    "RegisterDomainResponseTypeDef",
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "RenewDomainResponseTypeDef",
+    "ResendContactReachabilityEmailResponseTypeDef",
     "RetrieveDomainAuthCodeResponseTypeDef",
     "TransferDomainResponseTypeDef",
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
-    "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
-    "ViewBillingRequestRequestTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
+    "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
+    "ListPricesRequestListPricesPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    "ListOperationsRequestRequestTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
+    "NameserverUnionTypeDef",
     "GetDomainDetailResponseTypeDef",
+    "ContactDetailUnionTypeDef",
     "RegisterDomainRequestRequestTypeDef",
-    "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
+    "TransferDomainRequestRequestTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
 )
 
 AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
     },
 )
 
-AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DnssecSigningAttributesTypeDef = TypedDict(
     "DnssecSigningAttributesTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
     },
     total=False,
 )
 
-AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BillingRecordTypeDef = TypedDict(
     "BillingRecordTypeDef",
     {
         "DomainName": str,
         "Operation": OperationTypeType,
         "InvoiceId": str,
         "BillDate": datetime,
@@ -177,74 +176,54 @@
 CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_OptionalCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "IdnLangCode": str,
     },
     total=False,
 )
 
-
 class CheckDomainAvailabilityRequestRequestTypeDef(
     _RequiredCheckDomainAvailabilityRequestRequestTypeDef,
     _OptionalCheckDomainAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
-CheckDomainAvailabilityResponseTypeDef = TypedDict(
-    "CheckDomainAvailabilityResponseTypeDef",
-    {
-        "Availability": DomainAvailabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_OptionalCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "AuthCode": str,
     },
     total=False,
 )
 
-
 class CheckDomainTransferabilityRequestRequestTypeDef(
     _RequiredCheckDomainTransferabilityRequestRequestTypeDef,
     _OptionalCheckDomainTransferabilityRequestRequestTypeDef,
 ):
     pass
 
-
 DomainTransferabilityTypeDef = TypedDict(
     "DomainTransferabilityTypeDef",
     {
         "Transferable": TransferableType,
     },
     total=False,
 )
@@ -268,22 +247,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTagsForDomainRequestRequestTypeDef = TypedDict(
     "DeleteTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TagsToDelete": Sequence[str],
     },
 )
@@ -298,38 +269,22 @@
 DisableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "DisableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DisableDomainTransferLockResponseTypeDef = TypedDict(
-    "DisableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateDelegationSignerFromDomainRequestRequestTypeDef = TypedDict(
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Id": str,
     },
 )
 
-DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DnssecKeyTypeDef = TypedDict(
     "DnssecKeyTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
         "DigestType": int,
@@ -364,43 +319,28 @@
         "AutoRenew": bool,
         "TransferLock": bool,
         "Expiry": datetime,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableDomainAutoRenewRequestRequestTypeDef = TypedDict(
     "EnableDomainAutoRenewRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
 EnableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "EnableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-EnableDomainTransferLockResponseTypeDef = TypedDict(
-    "EnableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
@@ -410,49 +350,38 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
-GetContactReachabilityStatusResponseTypeDef = TypedDict(
-    "GetContactReachabilityStatusResponseTypeDef",
-    {
-        "domainName": str,
-        "status": ReachabilityStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-_RequiredNameserverTypeDef = TypedDict(
-    "_RequiredNameserverTypeDef",
+_RequiredNameserverOutputTypeDef = TypedDict(
+    "_RequiredNameserverOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalNameserverTypeDef = TypedDict(
-    "_OptionalNameserverTypeDef",
+_OptionalNameserverOutputTypeDef = TypedDict(
+    "_OptionalNameserverOutputTypeDef",
     {
         "GlueIps": List[str],
     },
     total=False,
 )
 
-
-class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+class NameserverOutputTypeDef(_RequiredNameserverOutputTypeDef, _OptionalNameserverOutputTypeDef):
     pass
 
-
 GetDomainSuggestionsRequestRequestTypeDef = TypedDict(
     "GetDomainSuggestionsRequestRequestTypeDef",
     {
         "DomainName": str,
         "SuggestionCount": int,
         "OnlyAvailable": bool,
     },
@@ -461,64 +390,33 @@
 GetOperationDetailRequestRequestTypeDef = TypedDict(
     "GetOperationDetailRequestRequestTypeDef",
     {
         "OperationId": str,
     },
 )
 
-GetOperationDetailResponseTypeDef = TypedDict(
-    "GetOperationDetailResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "OperationId": str,
-        "Status": OperationStatusType,
-        "Message": str,
-        "DomainName": str,
-        "Type": OperationTypeType,
-        "SubmittedDate": datetime,
-        "LastUpdatedDate": datetime,
-        "StatusFlag": StatusFlagType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortConditionTypeDef = TypedDict(
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListOperationsRequestRequestTypeDef = TypedDict(
-    "ListOperationsRequestRequestTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "OperationId": str,
         "Status": OperationStatusType,
         "Type": OperationTypeType,
         "SubmittedDate": datetime,
@@ -526,23 +424,14 @@
         "Message": str,
         "StatusFlag": StatusFlagType,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
-ListPricesRequestListPricesPaginateTypeDef = TypedDict(
-    "ListPricesRequestListPricesPaginateTypeDef",
-    {
-        "Tld": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPricesRequestRequestTypeDef = TypedDict(
     "ListPricesRequestRequestTypeDef",
     {
         "Tld": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -561,55 +450,46 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredNameserverTypeDef = TypedDict(
+    "_RequiredNameserverTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+    },
+)
+_OptionalNameserverTypeDef = TypedDict(
+    "_OptionalNameserverTypeDef",
+    {
+        "GlueIps": Sequence[str],
     },
     total=False,
 )
 
+class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+    pass
+
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
 
-RegisterDomainResponseTypeDef = TypedDict(
-    "RegisterDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRenewDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRenewDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "CurrentExpiryYear": int,
     },
 )
@@ -617,172 +497,247 @@
     "_OptionalRenewDomainRequestRequestTypeDef",
     {
         "DurationInYears": int,
     },
     total=False,
 )
 
-
 class RenewDomainRequestRequestTypeDef(
     _RequiredRenewDomainRequestRequestTypeDef, _OptionalRenewDomainRequestRequestTypeDef
 ):
     pass
 
+ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
+    "ResendContactReachabilityEmailRequestRequestTypeDef",
+    {
+        "domainName": str,
+    },
+    total=False,
+)
 
-RenewDomainResponseTypeDef = TypedDict(
-    "RenewDomainResponseTypeDef",
+ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
+    "ResendOperationAuthorizationRequestRequestTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
-    "ResendContactReachabilityEmailRequestRequestTypeDef",
+RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
-        "domainName": str,
+        "DomainName": str,
+    },
+)
+
+TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "AccountId": str,
+    },
+)
+
+_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
+    {
+        "AdminPrivacy": bool,
+        "RegistrantPrivacy": bool,
+        "TechPrivacy": bool,
     },
     total=False,
 )
 
-ResendContactReachabilityEmailResponseTypeDef = TypedDict(
-    "ResendContactReachabilityEmailResponseTypeDef",
+class UpdateDomainContactPrivacyRequestRequestTypeDef(
+    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
+    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
+):
+    pass
+
+AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
-        "domainName": str,
-        "emailAddress": str,
-        "isAlreadyVerified": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
-    "ResendOperationAuthorizationRequestRequestTypeDef",
+AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
+    "AssociateDelegationSignerToDomainResponseTypeDef",
     {
         "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeRequestRequestTypeDef",
+CheckDomainAvailabilityResponseTypeDef = TypedDict(
+    "CheckDomainAvailabilityResponseTypeDef",
     {
-        "DomainName": str,
+        "Availability": DomainAvailabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeResponseTypeDef",
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
     {
-        "AuthCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TransferDomainResponseTypeDef = TypedDict(
-    "TransferDomainResponseTypeDef",
+DisableDomainTransferLockResponseTypeDef = TypedDict(
+    "DisableDomainTransferLockResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     {
-        "DomainName": str,
-        "AccountId": str,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableDomainTransferLockResponseTypeDef = TypedDict(
+    "EnableDomainTransferLockResponseTypeDef",
     {
         "OperationId": str,
-        "Password": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
+GetContactReachabilityStatusResponseTypeDef = TypedDict(
+    "GetContactReachabilityStatusResponseTypeDef",
     {
+        "domainName": str,
+        "status": ReachabilityStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOperationDetailResponseTypeDef = TypedDict(
+    "GetOperationDetailResponseTypeDef",
+    {
+        "OperationId": str,
+        "Status": OperationStatusType,
+        "Message": str,
         "DomainName": str,
+        "Type": OperationTypeType,
+        "SubmittedDate": datetime,
+        "LastUpdatedDate": datetime,
+        "StatusFlag": StatusFlagType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
+
+RegisterDomainResponseTypeDef = TypedDict(
+    "RegisterDomainResponseTypeDef",
     {
-        "AdminPrivacy": bool,
-        "RegistrantPrivacy": bool,
-        "TechPrivacy": bool,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateDomainContactPrivacyRequestRequestTypeDef(
-    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
-    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
-):
-    pass
+RenewDomainResponseTypeDef = TypedDict(
+    "RenewDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ResendContactReachabilityEmailResponseTypeDef = TypedDict(
+    "ResendContactReachabilityEmailResponseTypeDef",
+    {
+        "domainName": str,
+        "emailAddress": str,
+        "isAlreadyVerified": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
-    "UpdateDomainContactPrivacyResponseTypeDef",
+RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeResponseTypeDef",
+    {
+        "AuthCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferDomainResponseTypeDef = TypedDict(
+    "TransferDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainContactResponseTypeDef = TypedDict(
-    "UpdateDomainContactResponseTypeDef",
+TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Password": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainNameserversResponseTypeDef = TypedDict(
-    "UpdateDomainNameserversResponseTypeDef",
+UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
+    "UpdateDomainContactPrivacyResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
+UpdateDomainContactResponseTypeDef = TypedDict(
+    "UpdateDomainContactResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
+UpdateDomainNameserversResponseTypeDef = TypedDict(
+    "UpdateDomainNameserversResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 AssociateDelegationSignerToDomainRequestRequestTypeDef = TypedDict(
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "SigningAttributes": DnssecSigningAttributesTypeDef,
@@ -790,26 +745,47 @@
 )
 
 ViewBillingResponseTypeDef = TypedDict(
     "ViewBillingResponseTypeDef",
     {
         "NextPageMarker": str,
         "BillingRecords": List[BillingRecordTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CheckDomainTransferabilityResponseTypeDef = TypedDict(
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContactDetailOutputTypeDef = TypedDict(
+    "ContactDetailOutputTypeDef",
+    {
+        "FirstName": str,
+        "LastName": str,
+        "ContactType": ContactTypeType,
+        "OrganizationName": str,
+        "AddressLine1": str,
+        "AddressLine2": str,
+        "City": str,
+        "State": str,
+        "CountryCode": CountryCodeType,
+        "ZipCode": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "Fax": str,
+        "ExtraParams": List[ExtraParamTypeDef],
+    },
+    total=False,
+)
+
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "ContactType": ContactTypeType,
         "OrganizationName": str,
@@ -818,15 +794,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": List[ExtraParamTypeDef],
+        "ExtraParams": Sequence[ExtraParamTypeDef],
     },
     total=False,
 )
 
 DomainPriceTypeDef = TypedDict(
     "DomainPriceTypeDef",
     {
@@ -840,56 +816,42 @@
     total=False,
 )
 
 GetDomainSuggestionsResponseTypeDef = TypedDict(
     "GetDomainSuggestionsResponseTypeDef",
     {
         "SuggestionsList": List[DomainSuggestionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
-    },
-)
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+ListPricesRequestListPricesPaginateTypeDef = TypedDict(
+    "ListPricesRequestListPricesPaginateTypeDef",
     {
-        "FIAuthKey": str,
+        "Tld": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
-):
-    pass
-
-
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
@@ -897,28 +859,76 @@
         "SortCondition": SortConditionTypeDef,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOperationsRequestRequestTypeDef = TypedDict(
+    "ListOperationsRequestRequestTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+    },
+    total=False,
+)
+
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+    },
+    total=False,
+)
+
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -928,31 +938,30 @@
     "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
     {
         "TagsToUpdate": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
-
+NameserverUnionTypeDef = Union[NameserverTypeDef, NameserverOutputTypeDef]
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
-        "Nameservers": List[NameserverTypeDef],
+        "Nameservers": List[NameserverOutputTypeDef],
         "AutoRenew": bool,
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
+        "AdminContact": ContactDetailOutputTypeDef,
+        "RegistrantContact": ContactDetailOutputTypeDef,
+        "TechContact": ContactDetailOutputTypeDef,
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
         "RegistrarName": str,
         "WhoIsServer": str,
         "RegistrarUrl": str,
         "AbuseContactEmail": str,
@@ -961,18 +970,19 @@
         "CreationDate": datetime,
         "UpdatedDate": datetime,
         "ExpirationDate": datetime,
         "Reseller": str,
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContactDetailUnionTypeDef = Union[ContactDetailTypeDef, ContactDetailOutputTypeDef]
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -987,20 +997,50 @@
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
-
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
+_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+    {
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
+        "Consent": ConsentTypeDef,
+    },
+    total=False,
+)
+
+class UpdateDomainContactRequestRequestTypeDef(
+    _RequiredUpdateDomainContactRequestRequestTypeDef,
+    _OptionalUpdateDomainContactRequestRequestTypeDef,
+):
+    pass
+
+ListPricesResponseTypeDef = TypedDict(
+    "ListPricesResponseTypeDef",
+    {
+        "Prices": List[DomainPriceTypeDef],
+        "NextPageMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
@@ -1008,57 +1048,42 @@
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "Nameservers": Sequence[NameserverUnionTypeDef],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
-
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
+        "Nameservers": Sequence[NameserverUnionTypeDef],
     },
 )
-_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
-        "Consent": ConsentTypeDef,
+        "FIAuthKey": str,
     },
     total=False,
 )
 
-
-class UpdateDomainContactRequestRequestTypeDef(
-    _RequiredUpdateDomainContactRequestRequestTypeDef,
-    _OptionalUpdateDomainContactRequestRequestTypeDef,
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
-
-
-ListPricesResponseTypeDef = TypedDict(
-    "ListPricesResponseTypeDef",
-    {
-        "Prices": List[DomainPriceTypeDef],
-        "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains/type_defs.pyi` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef
 
-    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = {...}
+    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,136 +35,137 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DnssecSigningAttributesTypeDef",
-    "AssociateDelegationSignerToDomainResponseTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
-    "CheckDomainAvailabilityResponseTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
-    "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     "DnssecKeyTypeDef",
     "PriceWithCurrencyTypeDef",
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
-    "EnableDomainTransferLockResponseTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
-    "GetContactReachabilityStatusResponseTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
-    "NameserverTypeDef",
+    "NameserverOutputTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
-    "GetOperationDetailResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    "ListOperationsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "OperationSummaryTypeDef",
-    "ListPricesRequestListPricesPaginateTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
-    "PaginatorConfigTypeDef",
+    "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
-    "RegisterDomainResponseTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "RenewDomainRequestRequestTypeDef",
-    "RenewDomainResponseTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
-    "ResendContactReachabilityEmailResponseTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+    "UpdateDomainContactPrivacyRequestRequestTypeDef",
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "AssociateDelegationSignerToDomainResponseTypeDef",
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+    "CheckDomainAvailabilityResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DisableDomainTransferLockResponseTypeDef",
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDomainTransferLockResponseTypeDef",
+    "GetContactReachabilityStatusResponseTypeDef",
+    "GetOperationDetailResponseTypeDef",
+    "RegisterDomainResponseTypeDef",
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "RenewDomainResponseTypeDef",
+    "ResendContactReachabilityEmailResponseTypeDef",
     "RetrieveDomainAuthCodeResponseTypeDef",
     "TransferDomainResponseTypeDef",
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
-    "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
-    "ViewBillingRequestRequestTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
+    "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
+    "ListPricesRequestListPricesPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    "ListOperationsRequestRequestTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
+    "NameserverUnionTypeDef",
     "GetDomainDetailResponseTypeDef",
+    "ContactDetailUnionTypeDef",
     "RegisterDomainRequestRequestTypeDef",
-    "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
+    "TransferDomainRequestRequestTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
 )
 
 AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
     },
 )
 
-AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DnssecSigningAttributesTypeDef = TypedDict(
     "DnssecSigningAttributesTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
     },
     total=False,
 )
 
-AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BillingRecordTypeDef = TypedDict(
     "BillingRecordTypeDef",
     {
         "DomainName": str,
         "Operation": OperationTypeType,
         "InvoiceId": str,
         "BillDate": datetime,
@@ -176,49 +177,35 @@
 CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_OptionalCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "IdnLangCode": str,
     },
     total=False,
 )
 
+
 class CheckDomainAvailabilityRequestRequestTypeDef(
     _RequiredCheckDomainAvailabilityRequestRequestTypeDef,
     _OptionalCheckDomainAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-CheckDomainAvailabilityResponseTypeDef = TypedDict(
-    "CheckDomainAvailabilityResponseTypeDef",
-    {
-        "Availability": DomainAvailabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
@@ -226,20 +213,22 @@
     "_OptionalCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "AuthCode": str,
     },
     total=False,
 )
 
+
 class CheckDomainTransferabilityRequestRequestTypeDef(
     _RequiredCheckDomainTransferabilityRequestRequestTypeDef,
     _OptionalCheckDomainTransferabilityRequestRequestTypeDef,
 ):
     pass
 
+
 DomainTransferabilityTypeDef = TypedDict(
     "DomainTransferabilityTypeDef",
     {
         "Transferable": TransferableType,
     },
     total=False,
 )
@@ -263,22 +252,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTagsForDomainRequestRequestTypeDef = TypedDict(
     "DeleteTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TagsToDelete": Sequence[str],
     },
 )
@@ -293,38 +274,22 @@
 DisableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "DisableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DisableDomainTransferLockResponseTypeDef = TypedDict(
-    "DisableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateDelegationSignerFromDomainRequestRequestTypeDef = TypedDict(
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Id": str,
     },
 )
 
-DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DnssecKeyTypeDef = TypedDict(
     "DnssecKeyTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
         "DigestType": int,
@@ -359,43 +324,28 @@
         "AutoRenew": bool,
         "TransferLock": bool,
         "Expiry": datetime,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableDomainAutoRenewRequestRequestTypeDef = TypedDict(
     "EnableDomainAutoRenewRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
 EnableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "EnableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-EnableDomainTransferLockResponseTypeDef = TypedDict(
-    "EnableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
@@ -405,47 +355,40 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
-GetContactReachabilityStatusResponseTypeDef = TypedDict(
-    "GetContactReachabilityStatusResponseTypeDef",
-    {
-        "domainName": str,
-        "status": ReachabilityStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-_RequiredNameserverTypeDef = TypedDict(
-    "_RequiredNameserverTypeDef",
+_RequiredNameserverOutputTypeDef = TypedDict(
+    "_RequiredNameserverOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalNameserverTypeDef = TypedDict(
-    "_OptionalNameserverTypeDef",
+_OptionalNameserverOutputTypeDef = TypedDict(
+    "_OptionalNameserverOutputTypeDef",
     {
         "GlueIps": List[str],
     },
     total=False,
 )
 
-class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+
+class NameserverOutputTypeDef(_RequiredNameserverOutputTypeDef, _OptionalNameserverOutputTypeDef):
     pass
 
+
 GetDomainSuggestionsRequestRequestTypeDef = TypedDict(
     "GetDomainSuggestionsRequestRequestTypeDef",
     {
         "DomainName": str,
         "SuggestionCount": int,
         "OnlyAvailable": bool,
     },
@@ -454,64 +397,33 @@
 GetOperationDetailRequestRequestTypeDef = TypedDict(
     "GetOperationDetailRequestRequestTypeDef",
     {
         "OperationId": str,
     },
 )
 
-GetOperationDetailResponseTypeDef = TypedDict(
-    "GetOperationDetailResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "OperationId": str,
-        "Status": OperationStatusType,
-        "Message": str,
-        "DomainName": str,
-        "Type": OperationTypeType,
-        "SubmittedDate": datetime,
-        "LastUpdatedDate": datetime,
-        "StatusFlag": StatusFlagType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortConditionTypeDef = TypedDict(
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListOperationsRequestRequestTypeDef = TypedDict(
-    "ListOperationsRequestRequestTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "OperationId": str,
         "Status": OperationStatusType,
         "Type": OperationTypeType,
         "SubmittedDate": datetime,
@@ -519,23 +431,14 @@
         "Message": str,
         "StatusFlag": StatusFlagType,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
-ListPricesRequestListPricesPaginateTypeDef = TypedDict(
-    "ListPricesRequestListPricesPaginateTypeDef",
-    {
-        "Tld": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPricesRequestRequestTypeDef = TypedDict(
     "ListPricesRequestRequestTypeDef",
     {
         "Tld": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -554,55 +457,48 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredNameserverTypeDef = TypedDict(
+    "_RequiredNameserverTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+    },
+)
+_OptionalNameserverTypeDef = TypedDict(
+    "_OptionalNameserverTypeDef",
+    {
+        "GlueIps": Sequence[str],
     },
     total=False,
 )
 
+
+class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+    pass
+
+
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
 
-RegisterDomainResponseTypeDef = TypedDict(
-    "RegisterDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRenewDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRenewDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "CurrentExpiryYear": int,
     },
 )
@@ -610,168 +506,251 @@
     "_OptionalRenewDomainRequestRequestTypeDef",
     {
         "DurationInYears": int,
     },
     total=False,
 )
 
+
 class RenewDomainRequestRequestTypeDef(
     _RequiredRenewDomainRequestRequestTypeDef, _OptionalRenewDomainRequestRequestTypeDef
 ):
     pass
 
-RenewDomainResponseTypeDef = TypedDict(
-    "RenewDomainResponseTypeDef",
+
+ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
+    "ResendContactReachabilityEmailRequestRequestTypeDef",
+    {
+        "domainName": str,
+    },
+    total=False,
+)
+
+ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
+    "ResendOperationAuthorizationRequestRequestTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
-    "ResendContactReachabilityEmailRequestRequestTypeDef",
+RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
-        "domainName": str,
+        "DomainName": str,
+    },
+)
+
+TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "AccountId": str,
+    },
+)
+
+_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
+    {
+        "AdminPrivacy": bool,
+        "RegistrantPrivacy": bool,
+        "TechPrivacy": bool,
     },
     total=False,
 )
 
-ResendContactReachabilityEmailResponseTypeDef = TypedDict(
-    "ResendContactReachabilityEmailResponseTypeDef",
+
+class UpdateDomainContactPrivacyRequestRequestTypeDef(
+    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
+    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
+):
+    pass
+
+
+AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
-        "domainName": str,
-        "emailAddress": str,
-        "isAlreadyVerified": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
-    "ResendOperationAuthorizationRequestRequestTypeDef",
+AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
+    "AssociateDelegationSignerToDomainResponseTypeDef",
     {
         "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeRequestRequestTypeDef",
+CheckDomainAvailabilityResponseTypeDef = TypedDict(
+    "CheckDomainAvailabilityResponseTypeDef",
     {
-        "DomainName": str,
+        "Availability": DomainAvailabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeResponseTypeDef",
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
     {
-        "AuthCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TransferDomainResponseTypeDef = TypedDict(
-    "TransferDomainResponseTypeDef",
+DisableDomainTransferLockResponseTypeDef = TypedDict(
+    "DisableDomainTransferLockResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     {
-        "DomainName": str,
-        "AccountId": str,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableDomainTransferLockResponseTypeDef = TypedDict(
+    "EnableDomainTransferLockResponseTypeDef",
     {
         "OperationId": str,
-        "Password": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
+GetContactReachabilityStatusResponseTypeDef = TypedDict(
+    "GetContactReachabilityStatusResponseTypeDef",
     {
+        "domainName": str,
+        "status": ReachabilityStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOperationDetailResponseTypeDef = TypedDict(
+    "GetOperationDetailResponseTypeDef",
+    {
+        "OperationId": str,
+        "Status": OperationStatusType,
+        "Message": str,
         "DomainName": str,
+        "Type": OperationTypeType,
+        "SubmittedDate": datetime,
+        "LastUpdatedDate": datetime,
+        "StatusFlag": StatusFlagType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
+
+RegisterDomainResponseTypeDef = TypedDict(
+    "RegisterDomainResponseTypeDef",
     {
-        "AdminPrivacy": bool,
-        "RegistrantPrivacy": bool,
-        "TechPrivacy": bool,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateDomainContactPrivacyRequestRequestTypeDef(
-    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
-    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
-):
-    pass
+RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
-    "UpdateDomainContactPrivacyResponseTypeDef",
+RenewDomainResponseTypeDef = TypedDict(
+    "RenewDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainContactResponseTypeDef = TypedDict(
-    "UpdateDomainContactResponseTypeDef",
+ResendContactReachabilityEmailResponseTypeDef = TypedDict(
+    "ResendContactReachabilityEmailResponseTypeDef",
+    {
+        "domainName": str,
+        "emailAddress": str,
+        "isAlreadyVerified": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeResponseTypeDef",
+    {
+        "AuthCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferDomainResponseTypeDef = TypedDict(
+    "TransferDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainNameserversResponseTypeDef = TypedDict(
-    "UpdateDomainNameserversResponseTypeDef",
+TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Password": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
+UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
+    "UpdateDomainContactPrivacyResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
+UpdateDomainContactResponseTypeDef = TypedDict(
+    "UpdateDomainContactResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainNameserversResponseTypeDef = TypedDict(
+    "UpdateDomainNameserversResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 AssociateDelegationSignerToDomainRequestRequestTypeDef = TypedDict(
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "SigningAttributes": DnssecSigningAttributesTypeDef,
@@ -779,26 +758,47 @@
 )
 
 ViewBillingResponseTypeDef = TypedDict(
     "ViewBillingResponseTypeDef",
     {
         "NextPageMarker": str,
         "BillingRecords": List[BillingRecordTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CheckDomainTransferabilityResponseTypeDef = TypedDict(
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContactDetailOutputTypeDef = TypedDict(
+    "ContactDetailOutputTypeDef",
+    {
+        "FirstName": str,
+        "LastName": str,
+        "ContactType": ContactTypeType,
+        "OrganizationName": str,
+        "AddressLine1": str,
+        "AddressLine2": str,
+        "City": str,
+        "State": str,
+        "CountryCode": CountryCodeType,
+        "ZipCode": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "Fax": str,
+        "ExtraParams": List[ExtraParamTypeDef],
+    },
+    total=False,
+)
+
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "ContactType": ContactTypeType,
         "OrganizationName": str,
@@ -807,15 +807,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": List[ExtraParamTypeDef],
+        "ExtraParams": Sequence[ExtraParamTypeDef],
     },
     total=False,
 )
 
 DomainPriceTypeDef = TypedDict(
     "DomainPriceTypeDef",
     {
@@ -829,54 +829,42 @@
     total=False,
 )
 
 GetDomainSuggestionsResponseTypeDef = TypedDict(
     "GetDomainSuggestionsResponseTypeDef",
     {
         "SuggestionsList": List[DomainSuggestionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
-    },
-)
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+ListPricesRequestListPricesPaginateTypeDef = TypedDict(
+    "ListPricesRequestListPricesPaginateTypeDef",
     {
-        "FIAuthKey": str,
+        "Tld": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
-):
-    pass
-
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
@@ -884,28 +872,76 @@
         "SortCondition": SortConditionTypeDef,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOperationsRequestRequestTypeDef = TypedDict(
+    "ListOperationsRequestRequestTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+    },
+    total=False,
+)
+
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+    },
+    total=False,
+)
+
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -915,29 +951,32 @@
     "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
     {
         "TagsToUpdate": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
+
+NameserverUnionTypeDef = Union[NameserverTypeDef, NameserverOutputTypeDef]
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
-        "Nameservers": List[NameserverTypeDef],
+        "Nameservers": List[NameserverOutputTypeDef],
         "AutoRenew": bool,
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
+        "AdminContact": ContactDetailOutputTypeDef,
+        "RegistrantContact": ContactDetailOutputTypeDef,
+        "TechContact": ContactDetailOutputTypeDef,
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
         "RegistrarName": str,
         "WhoIsServer": str,
         "RegistrarUrl": str,
         "AbuseContactEmail": str,
@@ -946,18 +985,19 @@
         "CreationDate": datetime,
         "UpdatedDate": datetime,
         "ExpirationDate": datetime,
         "Reseller": str,
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContactDetailUnionTypeDef = Union[ContactDetailTypeDef, ContactDetailOutputTypeDef]
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -972,72 +1012,100 @@
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
+
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+    {
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
+        "Consent": ConsentTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateDomainContactRequestRequestTypeDef(
+    _RequiredUpdateDomainContactRequestRequestTypeDef,
+    _OptionalUpdateDomainContactRequestRequestTypeDef,
+):
+    pass
+
+
+ListPricesResponseTypeDef = TypedDict(
+    "ListPricesResponseTypeDef",
+    {
+        "Prices": List[DomainPriceTypeDef],
+        "NextPageMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "Nameservers": Sequence[NameserverUnionTypeDef],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
+
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
+        "Nameservers": Sequence[NameserverUnionTypeDef],
     },
 )
-_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
-        "Consent": ConsentTypeDef,
+        "FIAuthKey": str,
     },
     total=False,
 )
 
-class UpdateDomainContactRequestRequestTypeDef(
-    _RequiredUpdateDomainContactRequestRequestTypeDef,
-    _OptionalUpdateDomainContactRequestRequestTypeDef,
+
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
-
-ListPricesResponseTypeDef = TypedDict(
-    "ListPricesResponseTypeDef",
-    {
-        "Prices": List[DomainPriceTypeDef],
-        "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/PKG-INFO` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53domains
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53Domains 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53Domains 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53domains type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53domains type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53domains"></a>
 
 # types-aiobotocore-route53domains
 
 [![PyPI - types-aiobotocore-route53domains](https://img.shields.io/pypi/v/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53domains?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53domains)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53domains)](https://pepy.tech/project/types-aiobotocore-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53Domains 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [types-aiobotocore-route53domains docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/).
 
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
@@ -329,112 +328,117 @@
 )
 
 
 def check_value(value: ContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53domains.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
-    NameserverTypeDef,
+    NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    GetOperationDetailResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListOperationsRequestRequestTypeDef,
+    TimestampTypeDef,
     OperationSummaryTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
-    PaginatorConfigTypeDef,
+    NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
-    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
-    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
+    GetOperationDetailResponseTypeDef,
+    RegisterDomainResponseTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    RenewDomainResponseTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListOperationsRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
+    NameserverUnionTypeDef,
     GetDomainDetailResponseTypeDef,
+    ContactDetailUnionTypeDef,
     RegisterDomainRequestRequestTypeDef,
-    TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
+    TransferDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
+def get_value() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53domains-2.5.2/types_aiobotocore_route53domains.egg-info/SOURCES.txt` & `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*


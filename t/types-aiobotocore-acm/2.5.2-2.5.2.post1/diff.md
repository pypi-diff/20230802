# Comparing `tmp/types-aiobotocore-acm-2.5.2.tar.gz` & `tmp/types-aiobotocore-acm-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
```

## Comparing `types-aiobotocore-acm-2.5.2.tar` & `types-aiobotocore-acm-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.841605 types-aiobotocore-acm-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-08 01:43:09.837605 types-aiobotocore-acm-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.841605 types-aiobotocore-acm-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-07-08 01:25:16.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-07-08 01:25:16.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-08 01:25:16.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-08 01:25:16.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-08 01:25:15.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.837605 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-08 01:43:09.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:09.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:09.000000 types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-2.5.2/LICENSE` & `types-aiobotocore-acm-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/PKG-INFO` & `types-aiobotocore-acm-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore acm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore acm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ACM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -347,45 +346,46 @@
 )
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_acm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_acm.type_defs import (
     TagTypeDef,
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
     ExpiryEventsConfigurationTypeDef,
-    ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
+    ExportCertificateRequestRequestTypeDef,
+    ImportCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
@@ -399,15 +399,15 @@
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-acm-2.5.2/README.md` & `types-aiobotocore-acm-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ACM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -314,45 +314,46 @@
 )
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_acm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_acm.type_defs import (
     TagTypeDef,
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
     ExpiryEventsConfigurationTypeDef,
-    ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
+    ExportCertificateRequestRequestTypeDef,
+    ImportCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
@@ -366,15 +367,15 @@
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-acm-2.5.2/setup.py` & `types-aiobotocore-acm-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore acm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore acm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_acm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/__init__.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/__init__.pyi` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/__main__.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACM 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ACM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/client.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
     session = get_session()
     async with session.create_client("acm") as client:
         client: ACMClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import CertificateStatusType, KeyAlgorithmType, SortOrderType, ValidationMethodType
 from .paginator import ListCertificatesPaginator
 from .type_defs import (
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     DescribeCertificateResponseTypeDef,
     DomainValidationOptionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateResponseTypeDef,
     FiltersTypeDef,
@@ -136,15 +136,15 @@
         Returns detailed metadata about the specified ACM certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.describe_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#describe_certificate)
         """
 
     async def export_certificate(
-        self, *, CertificateArn: str, Passphrase: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, CertificateArn: str, Passphrase: BlobTypeDef
     ) -> ExportCertificateResponseTypeDef:
         """
         Exports a private certificate issued by a private certificate authority (CA) for
         use anywhere.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.export_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#export_certificate)
@@ -180,18 +180,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#get_certificate)
         """
 
     async def import_certificate(
         self,
         *,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        PrivateKey: Union[str, bytes, IO[Any], StreamingBody],
+        Certificate: BlobTypeDef,
+        PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        CertificateChain: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
```

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/client.pyi` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
     session = get_session()
     async with session.create_client("acm") as client:
         client: ACMClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import CertificateStatusType, KeyAlgorithmType, SortOrderType, ValidationMethodType
 from .paginator import ListCertificatesPaginator
 from .type_defs import (
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     DescribeCertificateResponseTypeDef,
     DomainValidationOptionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateResponseTypeDef,
     FiltersTypeDef,
@@ -126,15 +126,15 @@
         """
         Returns detailed metadata about the specified ACM certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.describe_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#describe_certificate)
         """
     async def export_certificate(
-        self, *, CertificateArn: str, Passphrase: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, CertificateArn: str, Passphrase: BlobTypeDef
     ) -> ExportCertificateResponseTypeDef:
         """
         Exports a private certificate issued by a private certificate authority (CA) for
         use anywhere.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.export_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#export_certificate)
@@ -166,18 +166,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#get_certificate)
         """
     async def import_certificate(
         self,
         *,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        PrivateKey: Union[str, bytes, IO[Any], StreamingBody],
+        Certificate: BlobTypeDef,
+        PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        CertificateChain: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
```

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/literals.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/literals.pyi` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/paginator.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/paginator.pyi` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/type_defs.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_acm.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -41,35 +41,36 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
+    "BlobTypeDef",
     "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
     "ExpiryEventsConfigurationTypeDef",
-    "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
+    "ExportCertificateRequestRequestTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
@@ -101,14 +102,15 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CertificateOptionsTypeDef = TypedDict(
     "CertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
@@ -210,22 +212,14 @@
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
 
-ExportCertificateRequestRequestTypeDef = TypedDict(
-    "ExportCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Passphrase": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 FiltersTypeDef = TypedDict(
     "FiltersTypeDef",
     {
         "extendedKeyUsage": Sequence[ExtendedKeyUsageNameType],
         "keyUsage": Sequence[KeyUsageNameType],
         "keyTypes": Sequence[KeyAlgorithmType],
     },
@@ -276,46 +270,54 @@
     "AddTagsToCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+ExportCertificateRequestRequestTypeDef = TypedDict(
+    "ExportCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Passphrase": BlobTypeDef,
+    },
+)
+
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-        "PrivateKey": Union[str, bytes, IO[Any], StreamingBody],
+        "Certificate": BlobTypeDef,
+        "PrivateKey": BlobTypeDef,
     },
 )
 _OptionalImportCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalImportCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
+        "CertificateChain": BlobTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class ImportCertificateRequestRequestTypeDef(
     _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
 ):
     pass
 
 
-RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 UpdateCertificateOptionsRequestRequestTypeDef = TypedDict(
     "UpdateCertificateOptionsRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Options": CertificateOptionsTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/type_defs.pyi` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_acm.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -40,35 +40,36 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
+    "BlobTypeDef",
     "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
     "ExpiryEventsConfigurationTypeDef",
-    "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
+    "ExportCertificateRequestRequestTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
@@ -98,14 +99,15 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CertificateOptionsTypeDef = TypedDict(
     "CertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
@@ -207,22 +209,14 @@
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
 
-ExportCertificateRequestRequestTypeDef = TypedDict(
-    "ExportCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Passphrase": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 FiltersTypeDef = TypedDict(
     "FiltersTypeDef",
     {
         "extendedKeyUsage": Sequence[ExtendedKeyUsageNameType],
         "keyUsage": Sequence[KeyUsageNameType],
         "keyTypes": Sequence[KeyAlgorithmType],
     },
@@ -273,44 +267,52 @@
     "AddTagsToCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+ExportCertificateRequestRequestTypeDef = TypedDict(
+    "ExportCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Passphrase": BlobTypeDef,
+    },
+)
+
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-        "PrivateKey": Union[str, bytes, IO[Any], StreamingBody],
+        "Certificate": BlobTypeDef,
+        "PrivateKey": BlobTypeDef,
     },
 )
 _OptionalImportCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalImportCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
+        "CertificateChain": BlobTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class ImportCertificateRequestRequestTypeDef(
     _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
 ):
     pass
 
-RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 UpdateCertificateOptionsRequestRequestTypeDef = TypedDict(
     "UpdateCertificateOptionsRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Options": CertificateOptionsTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/waiter.py` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm/waiter.pyi` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/PKG-INFO` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore acm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore acm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ACM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -347,45 +346,46 @@
 )
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_acm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_acm.type_defs import (
     TagTypeDef,
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
     ExpiryEventsConfigurationTypeDef,
-    ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
+    ExportCertificateRequestRequestTypeDef,
+    ImportCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
@@ -399,15 +399,15 @@
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-acm-2.5.2/types_aiobotocore_acm.egg-info/SOURCES.txt` & `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


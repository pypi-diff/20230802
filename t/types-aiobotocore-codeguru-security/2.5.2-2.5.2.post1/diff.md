# Comparing `tmp/types-aiobotocore-codeguru-security-2.5.2.tar.gz` & `tmp/types-aiobotocore-codeguru-security-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-security-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-security-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-security-2.5.2.tar` & `types-aiobotocore-codeguru-security-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.865869 types-aiobotocore-codeguru-security-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-07-08 01:43:23.865869 types-aiobotocore-codeguru-security-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.865869 types-aiobotocore-codeguru-security-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-08 01:27:36.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-08 01:27:36.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-07-08 01:27:36.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.865869 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.673624 types-aiobotocore-codeguru-security-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-02 14:52:02.669624 types-aiobotocore-codeguru-security-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.673624 types-aiobotocore-codeguru-security-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.661625 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:35:10.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-08-02 14:35:09.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.669624 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/LICENSE` & `types-aiobotocore-codeguru-security-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2/PKG-INFO` & `types-aiobotocore-codeguru-security-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguru-security type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeguru-security type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguru-security"></a>
 
 # types-aiobotocore-codeguru-security
 
 [![PyPI - types-aiobotocore-codeguru-security](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-security?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-security)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruSecurity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
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
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
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
@@ -320,73 +319,74 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguru_security.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
+    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
+    TimestampTypeDef,
     GetScanRequestRequestTypeDef,
-    GetScanResponseTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    GetScanResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
+    GetMetricsSummaryRequestRequestTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    ListFindingsMetricsRequestRequestTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
     BatchGetFindingsResponseTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> FindingMetricsValuePerSeverityTypeDef:
+def get_value() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/README.md` & `types-aiobotocore-codeguru-security-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codeguru-security"></a>
 
 # types-aiobotocore-codeguru-security
 
 [![PyPI - types-aiobotocore-codeguru-security](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-security?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-security)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruSecurity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
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
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
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
@@ -287,73 +287,74 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguru_security.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
+    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
+    TimestampTypeDef,
     GetScanRequestRequestTypeDef,
-    GetScanResponseTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    GetScanResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
+    GetMetricsSummaryRequestRequestTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    ListFindingsMetricsRequestRequestTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
     BatchGetFindingsResponseTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> FindingMetricsValuePerSeverityTypeDef:
+def get_value() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/setup.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-security",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore codeguru-security type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore codeguru-security type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeguru_security": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/"
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/__init__.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/__init__.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/__main__.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
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

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/client.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("codeguru-security") as client:
         client: CodeGuruSecurityClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import AnalysisTypeType, ScanTypeType, StatusType
 from .paginator import GetFindingsPaginator, ListFindingsMetricsPaginator, ListScansPaginator
 from .type_defs import (
@@ -33,14 +32,15 @@
     GetFindingsResponseTypeDef,
     GetMetricsSummaryResponseTypeDef,
     GetScanResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ResourceIdTypeDef,
+    TimestampTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -169,15 +169,15 @@
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#get_findings)
         """
 
     async def get_metrics_summary(
-        self, *, date: Union[datetime, str]
+        self, *, date: TimestampTypeDef
     ) -> GetMetricsSummaryResponseTypeDef:
         """
         Returns top level metrics about an account from a specified date, including
         number of open findings, the categories with most findings, the scans with most
         open findings, and scans with most open critical findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_metrics_summary)
@@ -191,16 +191,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#get_scan)
         """
 
     async def list_findings_metrics(
         self,
         *,
-        endDate: Union[datetime, str],
-        startDate: Union[datetime, str],
+        endDate: TimestampTypeDef,
+        startDate: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/client.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("codeguru-security") as client:
         client: CodeGuruSecurityClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import AnalysisTypeType, ScanTypeType, StatusType
 from .paginator import GetFindingsPaginator, ListFindingsMetricsPaginator, ListScansPaginator
 from .type_defs import (
@@ -33,14 +32,15 @@
     GetFindingsResponseTypeDef,
     GetMetricsSummaryResponseTypeDef,
     GetScanResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ResourceIdTypeDef,
+    TimestampTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -156,15 +156,15 @@
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#get_findings)
         """
     async def get_metrics_summary(
-        self, *, date: Union[datetime, str]
+        self, *, date: TimestampTypeDef
     ) -> GetMetricsSummaryResponseTypeDef:
         """
         Returns top level metrics about an account from a specified date, including
         number of open findings, the categories with most findings, the scans with most
         open findings, and scans with most open critical findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_metrics_summary)
@@ -176,16 +176,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#get_scan)
         """
     async def list_findings_metrics(
         self,
         *,
-        endDate: Union[datetime, str],
-        startDate: Union[datetime, str],
+        endDate: TimestampTypeDef,
+        startDate: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/literals.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/literals.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/paginator.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,26 +20,26 @@
         client: CodeGuruSecurityClient
 
         get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
         list_findings_metrics_paginator: ListFindingsMetricsPaginator = client.get_paginator("list_findings_metrics")
         list_scans_paginator: ListScansPaginator = client.get_paginator("list_scans")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import StatusType
 from .type_defs import (
     GetFindingsResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("GetFindingsPaginator", "ListFindingsMetricsPaginator", "ListScansPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -58,15 +58,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#getfindingspaginator)
         """
 
 
@@ -75,30 +75,30 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listfindingsmetricspaginator)
     """
 
     def paginate(
         self,
         *,
-        endDate: Union[datetime, str],
-        startDate: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        endDate: TimestampTypeDef,
+        startDate: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 
 class ListScansPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listscanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listscanspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/paginator.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,26 @@
         client: CodeGuruSecurityClient
 
         get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
         list_findings_metrics_paginator: ListFindingsMetricsPaginator = client.get_paginator("list_findings_metrics")
         list_scans_paginator: ListScansPaginator = client.get_paginator("list_scans")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import StatusType
 from .type_defs import (
     GetFindingsResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("GetFindingsPaginator", "ListFindingsMetricsPaginator", "ListScansPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -55,15 +55,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#getfindingspaginator)
         """
 
 class ListFindingsMetricsPaginator(AioPaginator):
@@ -71,29 +71,29 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listfindingsmetricspaginator)
     """
 
     def paginate(
         self,
         *,
-        endDate: Union[datetime, str],
-        startDate: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        endDate: TimestampTypeDef,
+        startDate: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 class ListScansPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listscanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listscanspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/type_defs.py` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
-    data: FindingMetricsValuePerSeverityTypeDef = {...}
+    data: FindingMetricsValuePerSeverityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,48 +30,49 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
+    "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
-    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "GetMetricsSummaryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetScanRequestRequestTypeDef",
-    "GetScanResponseTypeDef",
-    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    "ListFindingsMetricsRequestRequestTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ScanNameWithFindingNumTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountFindingsMetricTypeDef",
     "BatchGetFindingsRequestRequestTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "GetScanResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
+    "GetMetricsSummaryRequestRequestTypeDef",
+    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    "ListFindingsMetricsRequestRequestTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -105,14 +106,25 @@
     "FindingIdentifierTypeDef",
     {
         "findingId": str,
         "scanName": str,
     },
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
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
     total=False,
@@ -138,24 +150,14 @@
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "codeArtifactId": str,
-        "requestHeaders": Dict[str, str],
-        "s3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
@@ -165,37 +167,24 @@
     {
         "id": str,
         "subResourceId": str,
     },
     total=False,
 )
 
-_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "scanName": str,
-    },
-)
-_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetFindingsRequestGetFindingsPaginateTypeDef(
-    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
-    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -211,21 +200,15 @@
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
 
-GetMetricsSummaryRequestRequestTypeDef = TypedDict(
-    "GetMetricsSummaryRequestRequestTypeDef",
-    {
-        "date": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredGetScanRequestRequestTypeDef = TypedDict(
     "_RequiredGetScanRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetScanRequestRequestTypeDef = TypedDict(
@@ -239,84 +222,14 @@
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
 
-GetScanResponseTypeDef = TypedDict(
-    "GetScanResponseTypeDef",
-    {
-        "analysisType": AnalysisTypeType,
-        "createdAt": datetime,
-        "numberOfRevisions": int,
-        "runId": str,
-        "scanName": str,
-        "scanNameArn": str,
-        "scanState": ScanStateType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
-    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestRequestTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListFindingsMetricsRequestRequestTypeDef(
-    _RequiredListFindingsMetricsRequestRequestTypeDef,
-    _OptionalListFindingsMetricsRequestRequestTypeDef,
-):
-    pass
-
-
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -348,41 +261,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
     total=False,
@@ -393,25 +288,14 @@
     {
         "code": str,
         "description": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -439,14 +323,47 @@
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
 )
 
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "codeArtifactId": str,
+        "requestHeaders": Dict[str, str],
+        "s3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetScanResponseTypeDef = TypedDict(
+    "GetScanResponseTypeDef",
+    {
+        "analysisType": AnalysisTypeType,
+        "createdAt": datetime,
+        "numberOfRevisions": int,
+        "runId": str,
+        "scanName": str,
+        "scanNameArn": str,
+        "scanState": ScanStateType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FilePathTypeDef = TypedDict(
     "FilePathTypeDef",
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
@@ -484,47 +401,132 @@
     "CreateScanResponseTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
     },
 )
 
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "scanName": str,
     },
 )
+_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetFindingsRequestGetFindingsPaginateTypeDef(
+    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
+    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
+):
+    pass
+
+
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetMetricsSummaryRequestRequestTypeDef = TypedDict(
+    "GetMetricsSummaryRequestRequestTypeDef",
+    {
+        "date": TimestampTypeDef,
+    },
+)
+
+_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "endDate": TimestampTypeDef,
+        "startDate": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
+    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestRequestTypeDef",
+    {
+        "endDate": TimestampTypeDef,
+        "startDate": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListFindingsMetricsRequestRequestTypeDef(
+    _RequiredListFindingsMetricsRequestRequestTypeDef,
+    _OptionalListFindingsMetricsRequestRequestTypeDef,
+):
+    pass
+
 
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsSummaryTypeDef = TypedDict(
     "MetricsSummaryTypeDef",
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
@@ -546,15 +548,15 @@
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "filePath": FilePathTypeDef,
@@ -566,15 +568,15 @@
     total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "createdAt": datetime,
@@ -598,19 +600,19 @@
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security/type_defs.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
-    data: FindingMetricsValuePerSeverityTypeDef = {...}
+    data: FindingMetricsValuePerSeverityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -29,48 +29,49 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
+    "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
-    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "GetMetricsSummaryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetScanRequestRequestTypeDef",
-    "GetScanResponseTypeDef",
-    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    "ListFindingsMetricsRequestRequestTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ScanNameWithFindingNumTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountFindingsMetricTypeDef",
     "BatchGetFindingsRequestRequestTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "GetScanResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
+    "GetMetricsSummaryRequestRequestTypeDef",
+    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    "ListFindingsMetricsRequestRequestTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -104,14 +105,25 @@
     "FindingIdentifierTypeDef",
     {
         "findingId": str,
         "scanName": str,
     },
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
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
     total=False,
@@ -137,24 +149,14 @@
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "codeArtifactId": str,
-        "requestHeaders": Dict[str, str],
-        "s3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
@@ -164,35 +166,24 @@
     {
         "id": str,
         "subResourceId": str,
     },
     total=False,
 )
 
-_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "scanName": str,
-    },
-)
-_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetFindingsRequestGetFindingsPaginateTypeDef(
-    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
-    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -206,21 +197,15 @@
 )
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
-GetMetricsSummaryRequestRequestTypeDef = TypedDict(
-    "GetMetricsSummaryRequestRequestTypeDef",
-    {
-        "date": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredGetScanRequestRequestTypeDef = TypedDict(
     "_RequiredGetScanRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetScanRequestRequestTypeDef = TypedDict(
@@ -232,80 +217,14 @@
 )
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
-GetScanResponseTypeDef = TypedDict(
-    "GetScanResponseTypeDef",
-    {
-        "analysisType": AnalysisTypeType,
-        "createdAt": datetime,
-        "numberOfRevisions": int,
-        "runId": str,
-        "scanName": str,
-        "scanNameArn": str,
-        "scanState": ScanStateType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
-    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestRequestTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListFindingsMetricsRequestRequestTypeDef(
-    _RequiredListFindingsMetricsRequestRequestTypeDef,
-    _OptionalListFindingsMetricsRequestRequestTypeDef,
-):
-    pass
-
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -335,41 +254,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
     total=False,
@@ -380,25 +281,14 @@
     {
         "code": str,
         "description": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -426,14 +316,47 @@
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
 )
 
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "codeArtifactId": str,
+        "requestHeaders": Dict[str, str],
+        "s3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetScanResponseTypeDef = TypedDict(
+    "GetScanResponseTypeDef",
+    {
+        "analysisType": AnalysisTypeType,
+        "createdAt": datetime,
+        "numberOfRevisions": int,
+        "runId": str,
+        "scanName": str,
+        "scanNameArn": str,
+        "scanState": ScanStateType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FilePathTypeDef = TypedDict(
     "FilePathTypeDef",
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
@@ -469,47 +392,126 @@
     "CreateScanResponseTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
     },
 )
 
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "scanName": str,
+    },
+)
+_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetFindingsRequestGetFindingsPaginateTypeDef(
+    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
+    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
+):
+    pass
+
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetMetricsSummaryRequestRequestTypeDef = TypedDict(
+    "GetMetricsSummaryRequestRequestTypeDef",
+    {
+        "date": TimestampTypeDef,
+    },
+)
+
+_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "endDate": TimestampTypeDef,
+        "startDate": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
+    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestRequestTypeDef",
+    {
+        "endDate": TimestampTypeDef,
+        "startDate": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListFindingsMetricsRequestRequestTypeDef(
+    _RequiredListFindingsMetricsRequestRequestTypeDef,
+    _OptionalListFindingsMetricsRequestRequestTypeDef,
+):
+    pass
+
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsSummaryTypeDef = TypedDict(
     "MetricsSummaryTypeDef",
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
@@ -531,15 +533,15 @@
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "filePath": FilePathTypeDef,
@@ -551,15 +553,15 @@
     total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "createdAt": datetime,
@@ -583,19 +585,19 @@
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguru-security type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeguru-security type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguru-security"></a>
 
 # types-aiobotocore-codeguru-security
 
 [![PyPI - types-aiobotocore-codeguru-security](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-security?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-security)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruSecurity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
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
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
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
@@ -320,73 +319,74 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguru_security.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
+    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
+    TimestampTypeDef,
     GetScanRequestRequestTypeDef,
-    GetScanResponseTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    GetScanResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
+    GetMetricsSummaryRequestRequestTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    ListFindingsMetricsRequestRequestTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
     BatchGetFindingsResponseTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> FindingMetricsValuePerSeverityTypeDef:
+def get_value() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*


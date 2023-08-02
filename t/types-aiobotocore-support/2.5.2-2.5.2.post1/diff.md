# Comparing `tmp/types-aiobotocore-support-2.5.2.tar.gz` & `tmp/types-aiobotocore-support-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-2.5.2.tar", last modified: Sat Jul  8 01:44:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
```

## Comparing `types-aiobotocore-support-2.5.2.tar` & `types-aiobotocore-support-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.558981 types-aiobotocore-support-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-08 01:44:24.554981 types-aiobotocore-support-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:24.558981 types-aiobotocore-support-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.542981 types-aiobotocore-support-2.5.2/types_aiobotocore_support/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16246 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-08 01:41:50.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-07-08 01:41:50.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-07-08 01:41:50.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18617 2023-07-08 01:41:50.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:49.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.554981 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-08 01:44:24.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:44:24.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:24.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:44:24.000000 types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-2.5.2/LICENSE` & `types-aiobotocore-support-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2/PKG-INFO` & `types-aiobotocore-support-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore support type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore support type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-support?color=blue)](https://pypistats.org/packages/types-aiobotocore-support)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Support 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
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
@@ -310,83 +309,86 @@
 )
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_support.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_support.type_defs import (
-    AttachmentTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
+    BlobTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
     DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
     DescribeSupportedLanguagesRequestRequestTypeDef,
     SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
-    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
-    ResolveCaseResponseTypeDef,
-    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeAttachmentResponseTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
+    AttachmentTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
+    AttachmentUnionTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
+    AddAttachmentsToSetRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-support-2.5.2/README.md` & `types-aiobotocore-support-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-support?color=blue)](https://pypistats.org/packages/types-aiobotocore-support)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Support 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
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
@@ -277,83 +277,86 @@
 )
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_support.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_support.type_defs import (
-    AttachmentTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
+    BlobTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
     DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
     DescribeSupportedLanguagesRequestRequestTypeDef,
     SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
-    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
-    ResolveCaseResponseTypeDef,
-    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeAttachmentResponseTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
+    AttachmentTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
+    AttachmentUnionTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
+    AddAttachmentsToSetRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-support-2.5.2/setup.py` & `types-aiobotocore-support-2.5.2.post1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore support type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore support type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_support": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/"
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/__init__.py` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/__init__.pyi` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/__main__.py` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Support 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Support 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/client.py` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentTypeDef,
+    AttachmentUnionTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -86,15 +86,15 @@
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#exceptions)
         """
 
     async def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#add_attachments_to_set)
         """
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/client.pyi` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentTypeDef,
+    AttachmentUnionTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -81,15 +81,15 @@
         """
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#exceptions)
         """
     async def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#add_attachments_to_set)
         """
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/literals.py` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/literals.pyi` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/paginator.py` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecasespaginator)
         """
 
 
@@ -78,13 +78,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/paginator.pyi` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecasespaginator)
         """
 
 class DescribeCommunicationsPaginator(AioPaginator):
@@ -74,13 +74,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/type_defs.py` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,104 +2,100 @@
 Type annotations for support service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_support.type_defs import AttachmentTypeDef
+    from types_aiobotocore_support.type_defs import ResponseMetadataTypeDef
 
-    data: AttachmentTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AttachmentTypeDef",
-    "AddAttachmentsToSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
-    "AddCommunicationToCaseResponseTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
+    "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
-    "CreateCaseResponseTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
-    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeCommunicationsRequestRequestTypeDef",
     "DescribeCreateCaseOptionsRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "DescribeSeverityLevelsRequestRequestTypeDef",
     "SeverityLevelTypeDef",
     "DescribeSupportedLanguagesRequestRequestTypeDef",
     "SupportedLanguageTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     "TrustedAdvisorCheckRefreshStatusTypeDef",
     "DescribeTrustedAdvisorCheckResultRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef",
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
-    "ResolveCaseResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
-    "DescribeAttachmentResponseTypeDef",
+    "AddAttachmentsToSetResponseTypeDef",
+    "AddCommunicationToCaseResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
+    "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
+    "AttachmentUnionTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
-AttachmentTypeDef = TypedDict(
-    "AttachmentTypeDef",
-    {
-        "fileName": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-AddAttachmentsToSetResponseTypeDef = TypedDict(
-    "AddAttachmentsToSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "attachmentSetId": str,
-        "expiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "_RequiredAddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
@@ -119,31 +115,33 @@
 class AddCommunicationToCaseRequestRequestTypeDef(
     _RequiredAddCommunicationToCaseRequestRequestTypeDef,
     _OptionalAddCommunicationToCaseRequestRequestTypeDef,
 ):
     pass
 
 
-AddCommunicationToCaseResponseTypeDef = TypedDict(
-    "AddCommunicationToCaseResponseTypeDef",
+AttachmentDetailsTypeDef = TypedDict(
+    "AttachmentDetailsTypeDef",
     {
-        "result": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attachmentId": str,
+        "fileName": str,
     },
+    total=False,
 )
 
-AttachmentDetailsTypeDef = TypedDict(
-    "AttachmentDetailsTypeDef",
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
     {
-        "attachmentId": str,
         "fileName": str,
+        "data": bytes,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
     total=False,
@@ -191,40 +189,27 @@
 
 class CreateCaseRequestRequestTypeDef(
     _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAttachmentRequestRequestTypeDef = TypedDict(
     "DescribeAttachmentRequestRequestTypeDef",
     {
         "attachmentId": str,
     },
 )
 
-DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "caseIdList": Sequence[str],
-        "displayId": str,
-        "afterTime": str,
-        "beforeTime": str,
-        "includeResolvedCases": bool,
-        "language": str,
-        "includeCommunications": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCasesRequestRequestTypeDef = TypedDict(
     "DescribeCasesRequestRequestTypeDef",
     {
@@ -237,38 +222,14 @@
         "maxResults": int,
         "language": str,
         "includeCommunications": bool,
     },
     total=False,
 )
 
-_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "caseId": str,
-    },
-)
-_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "beforeTime": str,
-        "afterTime": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
-    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCommunicationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommunicationsRequestRequestTypeDef",
     {
         "caseId": str,
     },
 )
 _OptionalDescribeCommunicationsRequestRequestTypeDef = TypedDict(
@@ -404,24 +365,14 @@
         "name": str,
         "description": str,
         "category": str,
         "metadata": List[str],
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
 RefreshTrustedAdvisorCheckRequestRequestTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     {
         "checkId": str,
     },
 )
 
@@ -429,34 +380,14 @@
     "ResolveCaseRequestRequestTypeDef",
     {
         "caseId": str,
     },
     total=False,
 )
 
-ResolveCaseResponseTypeDef = TypedDict(
-    "ResolveCaseResponseTypeDef",
-    {
-        "initialCaseStatus": str,
-        "finalCaseStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 TrustedAdvisorCostOptimizingSummaryTypeDef = TypedDict(
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     {
         "estimatedMonthlySavings": float,
         "estimatedPercentMonthlySavings": float,
     },
 )
@@ -491,41 +422,45 @@
         "resourcesProcessed": int,
         "resourcesFlagged": int,
         "resourcesIgnored": int,
         "resourcesSuppressed": int,
     },
 )
 
-_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+AddAttachmentsToSetResponseTypeDef = TypedDict(
+    "AddAttachmentsToSetResponseTypeDef",
     {
-        "attachments": Sequence[AttachmentTypeDef],
+        "attachmentSetId": str,
+        "expiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+
+AddCommunicationToCaseResponseTypeDef = TypedDict(
+    "AddCommunicationToCaseResponseTypeDef",
     {
-        "attachmentSetId": str,
+        "result": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AddAttachmentsToSetRequestRequestTypeDef(
-    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
-    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
-):
-    pass
-
-
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
+ResolveCaseResponseTypeDef = TypedDict(
+    "ResolveCaseResponseTypeDef",
     {
-        "attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "initialCaseStatus": str,
+        "finalCaseStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommunicationTypeDef = TypedDict(
     "CommunicationTypeDef",
     {
         "caseId": str,
@@ -533,14 +468,31 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachmentTypeDef = TypedDict(
+    "AttachmentTypeDef",
+    {
+        "fileName": str,
+        "data": BlobTypeDef,
+    },
+    total=False,
+)
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
@@ -553,51 +505,90 @@
         "type": str,
         "supportedHours": List[SupportedHourTypeDef],
         "datesWithoutSupport": List[DateIntervalTypeDef],
     },
     total=False,
 )
 
+DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    {
+        "caseIdList": Sequence[str],
+        "displayId": str,
+        "afterTime": str,
+        "beforeTime": str,
+        "includeResolvedCases": bool,
+        "language": str,
+        "includeCommunications": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "caseId": str,
+    },
+)
+_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "beforeTime": str,
+        "afterTime": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
+    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+):
+    pass
+
+
 DescribeSeverityLevelsResponseTypeDef = TypedDict(
     "DescribeSeverityLevelsResponseTypeDef",
     {
         "severityLevels": List[SeverityLevelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSupportedLanguagesResponseTypeDef = TypedDict(
     "DescribeSupportedLanguagesResponseTypeDef",
     {
         "supportedLanguages": List[SupportedLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     {
         "statuses": List[TrustedAdvisorCheckRefreshStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RefreshTrustedAdvisorCheckResponseTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     {
         "status": TrustedAdvisorCheckRefreshStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorChecksResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     {
         "checks": List[TrustedAdvisorCheckDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCategorySpecificSummaryTypeDef = TypedDict(
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     {
         "costOptimizing": TrustedAdvisorCostOptimizingSummaryTypeDef,
@@ -606,41 +597,42 @@
 )
 
 DescribeCommunicationsResponseTypeDef = TypedDict(
     "DescribeCommunicationsResponseTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
+AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCreateCaseOptionsResponseTypeDef = TypedDict(
     "DescribeCreateCaseOptionsResponseTypeDef",
     {
         "languageAvailability": str,
         "communicationTypes": List[CommunicationTypeOptionsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCheckResultTypeDef = TypedDict(
     "TrustedAdvisorCheckResultTypeDef",
     {
         "checkId": str,
@@ -692,31 +684,53 @@
         "recentCommunications": RecentCaseCommunicationsTypeDef,
         "ccEmailAddresses": List[str],
         "language": str,
     },
     total=False,
 )
 
+_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentUnionTypeDef],
+    },
+)
+_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachmentSetId": str,
+    },
+    total=False,
+)
+
+
+class AddAttachmentsToSetRequestRequestTypeDef(
+    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
+    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckSummariesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     {
         "summaries": List[TrustedAdvisorCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCasesResponseTypeDef = TypedDict(
     "DescribeCasesResponseTypeDef",
     {
         "cases": List[CaseDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support/type_defs.pyi` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,103 +2,99 @@
 Type annotations for support service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_support.type_defs import AttachmentTypeDef
+    from types_aiobotocore_support.type_defs import ResponseMetadataTypeDef
 
-    data: AttachmentTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AttachmentTypeDef",
-    "AddAttachmentsToSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
-    "AddCommunicationToCaseResponseTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
+    "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
-    "CreateCaseResponseTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
-    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeCommunicationsRequestRequestTypeDef",
     "DescribeCreateCaseOptionsRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "DescribeSeverityLevelsRequestRequestTypeDef",
     "SeverityLevelTypeDef",
     "DescribeSupportedLanguagesRequestRequestTypeDef",
     "SupportedLanguageTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     "TrustedAdvisorCheckRefreshStatusTypeDef",
     "DescribeTrustedAdvisorCheckResultRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef",
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
-    "ResolveCaseResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
-    "DescribeAttachmentResponseTypeDef",
+    "AddAttachmentsToSetResponseTypeDef",
+    "AddCommunicationToCaseResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
+    "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
+    "AttachmentUnionTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
-AttachmentTypeDef = TypedDict(
-    "AttachmentTypeDef",
-    {
-        "fileName": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-AddAttachmentsToSetResponseTypeDef = TypedDict(
-    "AddAttachmentsToSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "attachmentSetId": str,
-        "expiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "_RequiredAddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
@@ -116,31 +112,33 @@
 
 class AddCommunicationToCaseRequestRequestTypeDef(
     _RequiredAddCommunicationToCaseRequestRequestTypeDef,
     _OptionalAddCommunicationToCaseRequestRequestTypeDef,
 ):
     pass
 
-AddCommunicationToCaseResponseTypeDef = TypedDict(
-    "AddCommunicationToCaseResponseTypeDef",
+AttachmentDetailsTypeDef = TypedDict(
+    "AttachmentDetailsTypeDef",
     {
-        "result": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attachmentId": str,
+        "fileName": str,
     },
+    total=False,
 )
 
-AttachmentDetailsTypeDef = TypedDict(
-    "AttachmentDetailsTypeDef",
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
     {
-        "attachmentId": str,
         "fileName": str,
+        "data": bytes,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
     total=False,
@@ -186,40 +184,27 @@
 )
 
 class CreateCaseRequestRequestTypeDef(
     _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAttachmentRequestRequestTypeDef = TypedDict(
     "DescribeAttachmentRequestRequestTypeDef",
     {
         "attachmentId": str,
     },
 )
 
-DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "caseIdList": Sequence[str],
-        "displayId": str,
-        "afterTime": str,
-        "beforeTime": str,
-        "includeResolvedCases": bool,
-        "language": str,
-        "includeCommunications": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCasesRequestRequestTypeDef = TypedDict(
     "DescribeCasesRequestRequestTypeDef",
     {
@@ -232,36 +217,14 @@
         "maxResults": int,
         "language": str,
         "includeCommunications": bool,
     },
     total=False,
 )
 
-_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "caseId": str,
-    },
-)
-_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "beforeTime": str,
-        "afterTime": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
-    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCommunicationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommunicationsRequestRequestTypeDef",
     {
         "caseId": str,
     },
 )
 _OptionalDescribeCommunicationsRequestRequestTypeDef = TypedDict(
@@ -393,24 +356,14 @@
         "name": str,
         "description": str,
         "category": str,
         "metadata": List[str],
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
 RefreshTrustedAdvisorCheckRequestRequestTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     {
         "checkId": str,
     },
 )
 
@@ -418,34 +371,14 @@
     "ResolveCaseRequestRequestTypeDef",
     {
         "caseId": str,
     },
     total=False,
 )
 
-ResolveCaseResponseTypeDef = TypedDict(
-    "ResolveCaseResponseTypeDef",
-    {
-        "initialCaseStatus": str,
-        "finalCaseStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 TrustedAdvisorCostOptimizingSummaryTypeDef = TypedDict(
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     {
         "estimatedMonthlySavings": float,
         "estimatedPercentMonthlySavings": float,
     },
 )
@@ -478,39 +411,45 @@
         "resourcesProcessed": int,
         "resourcesFlagged": int,
         "resourcesIgnored": int,
         "resourcesSuppressed": int,
     },
 )
 
-_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+AddAttachmentsToSetResponseTypeDef = TypedDict(
+    "AddAttachmentsToSetResponseTypeDef",
     {
-        "attachments": Sequence[AttachmentTypeDef],
+        "attachmentSetId": str,
+        "expiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+
+AddCommunicationToCaseResponseTypeDef = TypedDict(
+    "AddCommunicationToCaseResponseTypeDef",
     {
-        "attachmentSetId": str,
+        "result": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AddAttachmentsToSetRequestRequestTypeDef(
-    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
-    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
-):
-    pass
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
+ResolveCaseResponseTypeDef = TypedDict(
+    "ResolveCaseResponseTypeDef",
     {
-        "attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "initialCaseStatus": str,
+        "finalCaseStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommunicationTypeDef = TypedDict(
     "CommunicationTypeDef",
     {
         "caseId": str,
@@ -518,14 +457,31 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachmentTypeDef = TypedDict(
+    "AttachmentTypeDef",
+    {
+        "fileName": str,
+        "data": BlobTypeDef,
+    },
+    total=False,
+)
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
@@ -538,51 +494,88 @@
         "type": str,
         "supportedHours": List[SupportedHourTypeDef],
         "datesWithoutSupport": List[DateIntervalTypeDef],
     },
     total=False,
 )
 
+DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    {
+        "caseIdList": Sequence[str],
+        "displayId": str,
+        "afterTime": str,
+        "beforeTime": str,
+        "includeResolvedCases": bool,
+        "language": str,
+        "includeCommunications": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "caseId": str,
+    },
+)
+_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "beforeTime": str,
+        "afterTime": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
+    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+):
+    pass
+
 DescribeSeverityLevelsResponseTypeDef = TypedDict(
     "DescribeSeverityLevelsResponseTypeDef",
     {
         "severityLevels": List[SeverityLevelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSupportedLanguagesResponseTypeDef = TypedDict(
     "DescribeSupportedLanguagesResponseTypeDef",
     {
         "supportedLanguages": List[SupportedLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     {
         "statuses": List[TrustedAdvisorCheckRefreshStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RefreshTrustedAdvisorCheckResponseTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     {
         "status": TrustedAdvisorCheckRefreshStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorChecksResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     {
         "checks": List[TrustedAdvisorCheckDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCategorySpecificSummaryTypeDef = TypedDict(
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     {
         "costOptimizing": TrustedAdvisorCostOptimizingSummaryTypeDef,
@@ -591,41 +584,42 @@
 )
 
 DescribeCommunicationsResponseTypeDef = TypedDict(
     "DescribeCommunicationsResponseTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
+AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCreateCaseOptionsResponseTypeDef = TypedDict(
     "DescribeCreateCaseOptionsResponseTypeDef",
     {
         "languageAvailability": str,
         "communicationTypes": List[CommunicationTypeOptionsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCheckResultTypeDef = TypedDict(
     "TrustedAdvisorCheckResultTypeDef",
     {
         "checkId": str,
@@ -675,31 +669,51 @@
         "recentCommunications": RecentCaseCommunicationsTypeDef,
         "ccEmailAddresses": List[str],
         "language": str,
     },
     total=False,
 )
 
+_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentUnionTypeDef],
+    },
+)
+_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachmentSetId": str,
+    },
+    total=False,
+)
+
+class AddAttachmentsToSetRequestRequestTypeDef(
+    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
+    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
+):
+    pass
+
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckSummariesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     {
         "summaries": List[TrustedAdvisorCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCasesResponseTypeDef = TypedDict(
     "DescribeCasesResponseTypeDef",
     {
         "cases": List[CaseDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/PKG-INFO` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore support type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore support type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-support?color=blue)](https://pypistats.org/packages/types-aiobotocore-support)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Support 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
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
@@ -310,83 +309,86 @@
 )
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_support.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_support.type_defs import (
-    AttachmentTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
+    BlobTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
     DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
     DescribeSupportedLanguagesRequestRequestTypeDef,
     SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
-    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
-    ResolveCaseResponseTypeDef,
-    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeAttachmentResponseTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
+    AttachmentTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
+    AttachmentUnionTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
+    AddAttachmentsToSetRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-support-2.5.2/types_aiobotocore_support.egg-info/SOURCES.txt` & `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*


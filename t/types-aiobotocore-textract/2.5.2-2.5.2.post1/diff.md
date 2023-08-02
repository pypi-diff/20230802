# Comparing `tmp/types-aiobotocore-textract-2.5.2.tar.gz` & `tmp/types-aiobotocore-textract-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-textract-2.5.2.tar", last modified: Sat Jul  8 01:44:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-textract-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
```

## Comparing `types-aiobotocore-textract-2.5.2.tar` & `types-aiobotocore-textract-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.150992 types-aiobotocore-textract-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-08 01:44:25.150992 types-aiobotocore-textract-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:25.150992 types-aiobotocore-textract-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.146992 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-08 01:41:58.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-07-08 01:41:58.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-08 01:41:58.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22967 2023-07-08 01:41:58.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-07-08 01:41:58.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:55.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.150992 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-08 01:44:24.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:44:25.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:24.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:24.000000 types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.865439 types-aiobotocore-textract-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-08-02 14:53:06.861439 types-aiobotocore-textract-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.865439 types-aiobotocore-textract-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.861439 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23383 2023-08-02 14:50:34.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.861439 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-textract-2.5.2/LICENSE` & `types-aiobotocore-textract-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2/PKG-INFO` & `types-aiobotocore-textract-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-textract
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Textract 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Textract 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore textract type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore textract type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-textract"></a>
 
 # types-aiobotocore-textract
 
 [![PyPI - types-aiobotocore-textract](https://img.shields.io/pypi/v/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-textract?color=blue)](https://pypistats.org/packages/types-aiobotocore-textract)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-textract)](https://pepy.tech/project/types-aiobotocore-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Textract 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [types-aiobotocore-textract docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -288,27 +287,29 @@
 )
 
 
 def check_value(value: BlockTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_textract.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
+    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
-    QueryTypeDef,
+    BlobTypeDef,
+    QueryOutputTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
     S3ObjectTypeDef,
     ExpenseCurrencyTypeDef,
@@ -321,41 +322,41 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
-    ResponseMetadataTypeDef,
+    QueryTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
-    QueriesConfigTypeDef,
     DocumentGroupTypeDef,
     DocumentLocationTypeDef,
     DocumentTypeDef,
     GeometryTypeDef,
     HumanLoopConfigTypeDef,
     PageClassificationTypeDef,
+    QueriesConfigTypeDef,
     IdentityDocumentFieldTypeDef,
     LendingSummaryTypeDef,
-    StartDocumentAnalysisRequestRequestTypeDef,
     StartDocumentTextDetectionRequestRequestTypeDef,
     StartExpenseAnalysisRequestRequestTypeDef,
     StartLendingAnalysisRequestRequestTypeDef,
     AnalyzeExpenseRequestRequestTypeDef,
     AnalyzeIDRequestRequestTypeDef,
     DetectDocumentTextRequestRequestTypeDef,
     BlockTypeDef,
     ExpenseDetectionTypeDef,
     LendingDetectionTypeDef,
     SignatureDetectionTypeDef,
     AnalyzeDocumentRequestRequestTypeDef,
+    StartDocumentAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryResponseTypeDef,
     AnalyzeDocumentResponseTypeDef,
     DetectDocumentTextResponseTypeDef,
     GetDocumentAnalysisResponseTypeDef,
     GetDocumentTextDetectionResponseTypeDef,
     IdentityDocumentTypeDef,
     ExpenseFieldTypeDef,
@@ -369,15 +370,15 @@
     ExtractionTypeDef,
     GetExpenseAnalysisResponseTypeDef,
     LendingResultTypeDef,
     GetLendingAnalysisResponseTypeDef,
 )
 
 
-def get_structure() -> DocumentMetadataTypeDef:
+def get_value() -> DocumentMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-textract-2.5.2/README.md` & `types-aiobotocore-textract-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-textract"></a>
 
 # types-aiobotocore-textract
 
 [![PyPI - types-aiobotocore-textract](https://img.shields.io/pypi/v/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-textract?color=blue)](https://pypistats.org/packages/types-aiobotocore-textract)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-textract)](https://pepy.tech/project/types-aiobotocore-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Textract 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [types-aiobotocore-textract docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -255,27 +255,29 @@
 )
 
 
 def check_value(value: BlockTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_textract.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
+    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
-    QueryTypeDef,
+    BlobTypeDef,
+    QueryOutputTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
     S3ObjectTypeDef,
     ExpenseCurrencyTypeDef,
@@ -288,41 +290,41 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
-    ResponseMetadataTypeDef,
+    QueryTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
-    QueriesConfigTypeDef,
     DocumentGroupTypeDef,
     DocumentLocationTypeDef,
     DocumentTypeDef,
     GeometryTypeDef,
     HumanLoopConfigTypeDef,
     PageClassificationTypeDef,
+    QueriesConfigTypeDef,
     IdentityDocumentFieldTypeDef,
     LendingSummaryTypeDef,
-    StartDocumentAnalysisRequestRequestTypeDef,
     StartDocumentTextDetectionRequestRequestTypeDef,
     StartExpenseAnalysisRequestRequestTypeDef,
     StartLendingAnalysisRequestRequestTypeDef,
     AnalyzeExpenseRequestRequestTypeDef,
     AnalyzeIDRequestRequestTypeDef,
     DetectDocumentTextRequestRequestTypeDef,
     BlockTypeDef,
     ExpenseDetectionTypeDef,
     LendingDetectionTypeDef,
     SignatureDetectionTypeDef,
     AnalyzeDocumentRequestRequestTypeDef,
+    StartDocumentAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryResponseTypeDef,
     AnalyzeDocumentResponseTypeDef,
     DetectDocumentTextResponseTypeDef,
     GetDocumentAnalysisResponseTypeDef,
     GetDocumentTextDetectionResponseTypeDef,
     IdentityDocumentTypeDef,
     ExpenseFieldTypeDef,
@@ -336,15 +338,15 @@
     ExtractionTypeDef,
     GetExpenseAnalysisResponseTypeDef,
     LendingResultTypeDef,
     GetLendingAnalysisResponseTypeDef,
 )
 
 
-def get_structure() -> DocumentMetadataTypeDef:
+def get_value() -> DocumentMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-textract-2.5.2/setup.py` & `types-aiobotocore-textract-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-textract",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_textract"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Textract 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore textract type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore textract type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_textract": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/"
```

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/__main__.py` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Textract 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Textract 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract\nOther"
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

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/client.py` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/client.pyi` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/literals.py` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/literals.pyi` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/type_defs.py` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_textract.type_defs import DocumentMetadataTypeDef
 
-    data: DocumentMetadataTypeDef = {...}
+    data: DocumentMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
@@ -36,16 +36,18 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
-    "QueryTypeDef",
+    "BlobTypeDef",
+    "QueryOutputTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
     "S3ObjectTypeDef",
     "ExpenseCurrencyTypeDef",
@@ -58,41 +60,41 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
-    "ResponseMetadataTypeDef",
+    "QueryTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
-    "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
     "DocumentLocationTypeDef",
     "DocumentTypeDef",
     "GeometryTypeDef",
     "HumanLoopConfigTypeDef",
     "PageClassificationTypeDef",
+    "QueriesConfigTypeDef",
     "IdentityDocumentFieldTypeDef",
     "LendingSummaryTypeDef",
-    "StartDocumentAnalysisRequestRequestTypeDef",
     "StartDocumentTextDetectionRequestRequestTypeDef",
     "StartExpenseAnalysisRequestRequestTypeDef",
     "StartLendingAnalysisRequestRequestTypeDef",
     "AnalyzeExpenseRequestRequestTypeDef",
     "AnalyzeIDRequestRequestTypeDef",
     "DetectDocumentTextRequestRequestTypeDef",
     "BlockTypeDef",
     "ExpenseDetectionTypeDef",
     "LendingDetectionTypeDef",
     "SignatureDetectionTypeDef",
     "AnalyzeDocumentRequestRequestTypeDef",
+    "StartDocumentAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryResponseTypeDef",
     "AnalyzeDocumentResponseTypeDef",
     "DetectDocumentTextResponseTypeDef",
     "GetDocumentAnalysisResponseTypeDef",
     "GetDocumentTextDetectionResponseTypeDef",
     "IdentityDocumentTypeDef",
     "ExpenseFieldTypeDef",
@@ -123,40 +125,52 @@
         "HumanLoopArn": str,
         "HumanLoopActivationReasons": List[str],
         "HumanLoopActivationConditionsEvaluationResults": str,
     },
     total=False,
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
 NormalizedValueTypeDef = TypedDict(
     "NormalizedValueTypeDef",
     {
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
 )
 
-_RequiredQueryTypeDef = TypedDict(
-    "_RequiredQueryTypeDef",
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredQueryOutputTypeDef = TypedDict(
+    "_RequiredQueryOutputTypeDef",
     {
         "Text": str,
     },
 )
-_OptionalQueryTypeDef = TypedDict(
-    "_OptionalQueryTypeDef",
+_OptionalQueryOutputTypeDef = TypedDict(
+    "_OptionalQueryOutputTypeDef",
     {
         "Alias": str,
-        "Pages": Sequence[str],
+        "Pages": List[str],
     },
     total=False,
 )
 
 
-class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+class QueryOutputTypeDef(_RequiredQueryOutputTypeDef, _OptionalQueryOutputTypeDef):
     pass
 
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "Type": RelationshipTypeType,
@@ -395,54 +409,63 @@
     {
         "Value": str,
         "Confidence": float,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredQueryTypeDef = TypedDict(
+    "_RequiredQueryTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Text": str,
     },
 )
+_OptionalQueryTypeDef = TypedDict(
+    "_OptionalQueryTypeDef",
+    {
+        "Alias": str,
+        "Pages": Sequence[str],
+    },
+    total=False,
+)
+
+
+class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+    pass
+
 
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDocumentTextDetectionResponseTypeDef = TypedDict(
     "StartDocumentTextDetectionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExpenseAnalysisResponseTypeDef = TypedDict(
     "StartExpenseAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLendingAnalysisResponseTypeDef = TypedDict(
     "StartLendingAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAnalyzeIDDetectionsTypeDef = TypedDict(
     "_RequiredAnalyzeIDDetectionsTypeDef",
     {
         "Text": str,
@@ -460,21 +483,14 @@
 
 class AnalyzeIDDetectionsTypeDef(
     _RequiredAnalyzeIDDetectionsTypeDef, _OptionalAnalyzeIDDetectionsTypeDef
 ):
     pass
 
 
-QueriesConfigTypeDef = TypedDict(
-    "QueriesConfigTypeDef",
-    {
-        "Queries": Sequence[QueryTypeDef],
-    },
-)
-
 DocumentGroupTypeDef = TypedDict(
     "DocumentGroupTypeDef",
     {
         "Type": str,
         "SplitDocuments": List[SplitDocumentTypeDef],
         "DetectedSignatures": List[DetectedSignatureTypeDef],
         "UndetectedSignatures": List[UndetectedSignatureTypeDef],
@@ -489,15 +505,15 @@
     },
     total=False,
 )
 
 DocumentTypeDef = TypedDict(
     "DocumentTypeDef",
     {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
@@ -532,14 +548,21 @@
     "PageClassificationTypeDef",
     {
         "PageType": List[PredictionTypeDef],
         "PageNumber": List[PredictionTypeDef],
     },
 )
 
+QueriesConfigTypeDef = TypedDict(
+    "QueriesConfigTypeDef",
+    {
+        "Queries": Sequence[QueryTypeDef],
+    },
+)
+
 IdentityDocumentFieldTypeDef = TypedDict(
     "IdentityDocumentFieldTypeDef",
     {
         "Type": AnalyzeIDDetectionsTypeDef,
         "ValueDetection": AnalyzeIDDetectionsTypeDef,
     },
     total=False,
@@ -550,42 +573,14 @@
     {
         "DocumentGroups": List[DocumentGroupTypeDef],
         "UndetectedDocumentTypes": List[str],
     },
     total=False,
 )
 
-_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "DocumentLocation": DocumentLocationTypeDef,
-        "FeatureTypes": Sequence[FeatureTypeType],
-    },
-)
-_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "JobTag": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "KMSKeyId": str,
-        "QueriesConfig": QueriesConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class StartDocumentAnalysisRequestRequestTypeDef(
-    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
-    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentTextDetectionRequestRequestTypeDef",
     {
         "DocumentLocation": DocumentLocationTypeDef,
     },
 )
 _OptionalStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
@@ -694,15 +689,15 @@
         "ColumnSpan": int,
         "Geometry": GeometryTypeDef,
         "Id": str,
         "Relationships": List[RelationshipTypeDef],
         "EntityTypes": List[EntityTypeType],
         "SelectionStatus": SelectionStatusType,
         "Page": int,
-        "Query": QueryTypeDef,
+        "Query": QueryOutputTypeDef,
     },
     total=False,
 )
 
 ExpenseDetectionTypeDef = TypedDict(
     "ExpenseDetectionTypeDef",
     {
@@ -752,73 +747,101 @@
 
 class AnalyzeDocumentRequestRequestTypeDef(
     _RequiredAnalyzeDocumentRequestRequestTypeDef, _OptionalAnalyzeDocumentRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "DocumentLocation": DocumentLocationTypeDef,
+        "FeatureTypes": Sequence[FeatureTypeType],
+    },
+)
+_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "JobTag": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
+        "KMSKeyId": str,
+        "QueriesConfig": QueriesConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class StartDocumentAnalysisRequestRequestTypeDef(
+    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
+    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
+):
+    pass
+
+
 GetLendingAnalysisSummaryResponseTypeDef = TypedDict(
     "GetLendingAnalysisSummaryResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalyzeDocumentResponseTypeDef = TypedDict(
     "AnalyzeDocumentResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectDocumentTextResponseTypeDef = TypedDict(
     "DetectDocumentTextResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentAnalysisResponseTypeDef = TypedDict(
     "GetDocumentAnalysisResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentTextDetectionResponseTypeDef = TypedDict(
     "GetDocumentTextDetectionResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityDocumentTypeDef = TypedDict(
     "IdentityDocumentTypeDef",
     {
         "DocumentIndex": int,
@@ -853,15 +876,15 @@
 
 AnalyzeIDResponseTypeDef = TypedDict(
     "AnalyzeIDResponseTypeDef",
     {
         "IdentityDocuments": List[IdentityDocumentTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "AnalyzeIDModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemFieldsTypeDef = TypedDict(
     "LineItemFieldsTypeDef",
     {
         "LineItemExpenseFields": List[ExpenseFieldTypeDef],
@@ -899,15 +922,15 @@
 )
 
 AnalyzeExpenseResponseTypeDef = TypedDict(
     "AnalyzeExpenseResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtractionTypeDef = TypedDict(
     "ExtractionTypeDef",
     {
         "LendingDocument": LendingDocumentTypeDef,
@@ -923,15 +946,15 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeExpenseModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LendingResultTypeDef = TypedDict(
     "LendingResultTypeDef",
     {
         "Page": int,
@@ -947,10 +970,10 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Results": List[LendingResultTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract/type_defs.pyi` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_textract.type_defs import DocumentMetadataTypeDef
 
-    data: DocumentMetadataTypeDef = {...}
+    data: DocumentMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
@@ -35,16 +35,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
-    "QueryTypeDef",
+    "BlobTypeDef",
+    "QueryOutputTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
     "S3ObjectTypeDef",
     "ExpenseCurrencyTypeDef",
@@ -57,41 +59,41 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
-    "ResponseMetadataTypeDef",
+    "QueryTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
-    "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
     "DocumentLocationTypeDef",
     "DocumentTypeDef",
     "GeometryTypeDef",
     "HumanLoopConfigTypeDef",
     "PageClassificationTypeDef",
+    "QueriesConfigTypeDef",
     "IdentityDocumentFieldTypeDef",
     "LendingSummaryTypeDef",
-    "StartDocumentAnalysisRequestRequestTypeDef",
     "StartDocumentTextDetectionRequestRequestTypeDef",
     "StartExpenseAnalysisRequestRequestTypeDef",
     "StartLendingAnalysisRequestRequestTypeDef",
     "AnalyzeExpenseRequestRequestTypeDef",
     "AnalyzeIDRequestRequestTypeDef",
     "DetectDocumentTextRequestRequestTypeDef",
     "BlockTypeDef",
     "ExpenseDetectionTypeDef",
     "LendingDetectionTypeDef",
     "SignatureDetectionTypeDef",
     "AnalyzeDocumentRequestRequestTypeDef",
+    "StartDocumentAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryResponseTypeDef",
     "AnalyzeDocumentResponseTypeDef",
     "DetectDocumentTextResponseTypeDef",
     "GetDocumentAnalysisResponseTypeDef",
     "GetDocumentTextDetectionResponseTypeDef",
     "IdentityDocumentTypeDef",
     "ExpenseFieldTypeDef",
@@ -122,39 +124,51 @@
         "HumanLoopArn": str,
         "HumanLoopActivationReasons": List[str],
         "HumanLoopActivationConditionsEvaluationResults": str,
     },
     total=False,
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
 NormalizedValueTypeDef = TypedDict(
     "NormalizedValueTypeDef",
     {
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
 )
 
-_RequiredQueryTypeDef = TypedDict(
-    "_RequiredQueryTypeDef",
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredQueryOutputTypeDef = TypedDict(
+    "_RequiredQueryOutputTypeDef",
     {
         "Text": str,
     },
 )
-_OptionalQueryTypeDef = TypedDict(
-    "_OptionalQueryTypeDef",
+_OptionalQueryOutputTypeDef = TypedDict(
+    "_OptionalQueryOutputTypeDef",
     {
         "Alias": str,
-        "Pages": Sequence[str],
+        "Pages": List[str],
     },
     total=False,
 )
 
-class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+class QueryOutputTypeDef(_RequiredQueryOutputTypeDef, _OptionalQueryOutputTypeDef):
     pass
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "Type": RelationshipTypeType,
         "Ids": List[str],
@@ -382,54 +396,61 @@
     {
         "Value": str,
         "Confidence": float,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredQueryTypeDef = TypedDict(
+    "_RequiredQueryTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Text": str,
+    },
+)
+_OptionalQueryTypeDef = TypedDict(
+    "_OptionalQueryTypeDef",
+    {
+        "Alias": str,
+        "Pages": Sequence[str],
     },
+    total=False,
 )
 
+class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+    pass
+
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDocumentTextDetectionResponseTypeDef = TypedDict(
     "StartDocumentTextDetectionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExpenseAnalysisResponseTypeDef = TypedDict(
     "StartExpenseAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLendingAnalysisResponseTypeDef = TypedDict(
     "StartLendingAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAnalyzeIDDetectionsTypeDef = TypedDict(
     "_RequiredAnalyzeIDDetectionsTypeDef",
     {
         "Text": str,
@@ -445,21 +466,14 @@
 )
 
 class AnalyzeIDDetectionsTypeDef(
     _RequiredAnalyzeIDDetectionsTypeDef, _OptionalAnalyzeIDDetectionsTypeDef
 ):
     pass
 
-QueriesConfigTypeDef = TypedDict(
-    "QueriesConfigTypeDef",
-    {
-        "Queries": Sequence[QueryTypeDef],
-    },
-)
-
 DocumentGroupTypeDef = TypedDict(
     "DocumentGroupTypeDef",
     {
         "Type": str,
         "SplitDocuments": List[SplitDocumentTypeDef],
         "DetectedSignatures": List[DetectedSignatureTypeDef],
         "UndetectedSignatures": List[UndetectedSignatureTypeDef],
@@ -474,15 +488,15 @@
     },
     total=False,
 )
 
 DocumentTypeDef = TypedDict(
     "DocumentTypeDef",
     {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
@@ -515,14 +529,21 @@
     "PageClassificationTypeDef",
     {
         "PageType": List[PredictionTypeDef],
         "PageNumber": List[PredictionTypeDef],
     },
 )
 
+QueriesConfigTypeDef = TypedDict(
+    "QueriesConfigTypeDef",
+    {
+        "Queries": Sequence[QueryTypeDef],
+    },
+)
+
 IdentityDocumentFieldTypeDef = TypedDict(
     "IdentityDocumentFieldTypeDef",
     {
         "Type": AnalyzeIDDetectionsTypeDef,
         "ValueDetection": AnalyzeIDDetectionsTypeDef,
     },
     total=False,
@@ -533,40 +554,14 @@
     {
         "DocumentGroups": List[DocumentGroupTypeDef],
         "UndetectedDocumentTypes": List[str],
     },
     total=False,
 )
 
-_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "DocumentLocation": DocumentLocationTypeDef,
-        "FeatureTypes": Sequence[FeatureTypeType],
-    },
-)
-_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "JobTag": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "KMSKeyId": str,
-        "QueriesConfig": QueriesConfigTypeDef,
-    },
-    total=False,
-)
-
-class StartDocumentAnalysisRequestRequestTypeDef(
-    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
-    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
-):
-    pass
-
 _RequiredStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentTextDetectionRequestRequestTypeDef",
     {
         "DocumentLocation": DocumentLocationTypeDef,
     },
 )
 _OptionalStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
@@ -669,15 +664,15 @@
         "ColumnSpan": int,
         "Geometry": GeometryTypeDef,
         "Id": str,
         "Relationships": List[RelationshipTypeDef],
         "EntityTypes": List[EntityTypeType],
         "SelectionStatus": SelectionStatusType,
         "Page": int,
-        "Query": QueryTypeDef,
+        "Query": QueryOutputTypeDef,
     },
     total=False,
 )
 
 ExpenseDetectionTypeDef = TypedDict(
     "ExpenseDetectionTypeDef",
     {
@@ -725,73 +720,99 @@
 )
 
 class AnalyzeDocumentRequestRequestTypeDef(
     _RequiredAnalyzeDocumentRequestRequestTypeDef, _OptionalAnalyzeDocumentRequestRequestTypeDef
 ):
     pass
 
+_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "DocumentLocation": DocumentLocationTypeDef,
+        "FeatureTypes": Sequence[FeatureTypeType],
+    },
+)
+_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "JobTag": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
+        "KMSKeyId": str,
+        "QueriesConfig": QueriesConfigTypeDef,
+    },
+    total=False,
+)
+
+class StartDocumentAnalysisRequestRequestTypeDef(
+    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
+    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
+):
+    pass
+
 GetLendingAnalysisSummaryResponseTypeDef = TypedDict(
     "GetLendingAnalysisSummaryResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalyzeDocumentResponseTypeDef = TypedDict(
     "AnalyzeDocumentResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectDocumentTextResponseTypeDef = TypedDict(
     "DetectDocumentTextResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentAnalysisResponseTypeDef = TypedDict(
     "GetDocumentAnalysisResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentTextDetectionResponseTypeDef = TypedDict(
     "GetDocumentTextDetectionResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityDocumentTypeDef = TypedDict(
     "IdentityDocumentTypeDef",
     {
         "DocumentIndex": int,
@@ -826,15 +847,15 @@
 
 AnalyzeIDResponseTypeDef = TypedDict(
     "AnalyzeIDResponseTypeDef",
     {
         "IdentityDocuments": List[IdentityDocumentTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "AnalyzeIDModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemFieldsTypeDef = TypedDict(
     "LineItemFieldsTypeDef",
     {
         "LineItemExpenseFields": List[ExpenseFieldTypeDef],
@@ -872,15 +893,15 @@
 )
 
 AnalyzeExpenseResponseTypeDef = TypedDict(
     "AnalyzeExpenseResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtractionTypeDef = TypedDict(
     "ExtractionTypeDef",
     {
         "LendingDocument": LendingDocumentTypeDef,
@@ -896,15 +917,15 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeExpenseModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LendingResultTypeDef = TypedDict(
     "LendingResultTypeDef",
     {
         "Page": int,
@@ -920,10 +941,10 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Results": List[LendingResultTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/PKG-INFO` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-textract
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Textract 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Textract 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore textract type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore textract type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-textract"></a>
 
 # types-aiobotocore-textract
 
 [![PyPI - types-aiobotocore-textract](https://img.shields.io/pypi/v/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-textract?color=blue)](https://pypistats.org/packages/types-aiobotocore-textract)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-textract)](https://pepy.tech/project/types-aiobotocore-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Textract 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [types-aiobotocore-textract docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -288,27 +287,29 @@
 )
 
 
 def check_value(value: BlockTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_textract.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
+    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
-    QueryTypeDef,
+    BlobTypeDef,
+    QueryOutputTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
     S3ObjectTypeDef,
     ExpenseCurrencyTypeDef,
@@ -321,41 +322,41 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
-    ResponseMetadataTypeDef,
+    QueryTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
-    QueriesConfigTypeDef,
     DocumentGroupTypeDef,
     DocumentLocationTypeDef,
     DocumentTypeDef,
     GeometryTypeDef,
     HumanLoopConfigTypeDef,
     PageClassificationTypeDef,
+    QueriesConfigTypeDef,
     IdentityDocumentFieldTypeDef,
     LendingSummaryTypeDef,
-    StartDocumentAnalysisRequestRequestTypeDef,
     StartDocumentTextDetectionRequestRequestTypeDef,
     StartExpenseAnalysisRequestRequestTypeDef,
     StartLendingAnalysisRequestRequestTypeDef,
     AnalyzeExpenseRequestRequestTypeDef,
     AnalyzeIDRequestRequestTypeDef,
     DetectDocumentTextRequestRequestTypeDef,
     BlockTypeDef,
     ExpenseDetectionTypeDef,
     LendingDetectionTypeDef,
     SignatureDetectionTypeDef,
     AnalyzeDocumentRequestRequestTypeDef,
+    StartDocumentAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryResponseTypeDef,
     AnalyzeDocumentResponseTypeDef,
     DetectDocumentTextResponseTypeDef,
     GetDocumentAnalysisResponseTypeDef,
     GetDocumentTextDetectionResponseTypeDef,
     IdentityDocumentTypeDef,
     ExpenseFieldTypeDef,
@@ -369,15 +370,15 @@
     ExtractionTypeDef,
     GetExpenseAnalysisResponseTypeDef,
     LendingResultTypeDef,
     GetLendingAnalysisResponseTypeDef,
 )
 
 
-def get_structure() -> DocumentMetadataTypeDef:
+def get_value() -> DocumentMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-textract-2.5.2/types_aiobotocore_textract.egg-info/SOURCES.txt` & `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/SOURCES.txt`

 * *Files identical despite different names*


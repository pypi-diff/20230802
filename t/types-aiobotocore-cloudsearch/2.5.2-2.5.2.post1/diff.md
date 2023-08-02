# Comparing `tmp/types-aiobotocore-cloudsearch-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudsearch-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
```

## Comparing `types-aiobotocore-cloudsearch-2.5.2.tar` & `types-aiobotocore-cloudsearch-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.649827 types-aiobotocore-cloudsearch-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-08 01:43:21.641827 types-aiobotocore-cloudsearch-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.649827 types-aiobotocore-cloudsearch-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.637827 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25526 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.641827 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.189636 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-08-02 14:34:42.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/LICENSE` & `types-aiobotocore-cloudsearch-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2/PKG-INFO` & `types-aiobotocore-cloudsearch-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudsearch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudsearch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudsearch"></a>
 
 # types-aiobotocore-cloudsearch
 
 [![PyPI - types-aiobotocore-cloudsearch](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearch)](https://pepy.tech/project/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [types-aiobotocore-cloudsearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/).
 
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
@@ -287,27 +286,27 @@
 )
 
 
 def check_value(value: AlgorithmicStemmingType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudsearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudsearch.type_defs import (
     OptionStatusTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    BuildSuggestersResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDomainRequestRequestTypeDef,
     DateArrayOptionsTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
@@ -325,30 +324,30 @@
     DocumentSuggesterOptionsTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
     DoubleArrayOptionsTypeDef,
     DoubleOptionsTypeDef,
     IndexDocumentsRequestRequestTypeDef,
-    IndexDocumentsResponseTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
-    ListDomainNamesResponseTypeDef,
-    ResponseMetadataTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
     AnalysisSchemeTypeDef,
+    BuildSuggestersResponseTypeDef,
+    IndexDocumentsResponseTypeDef,
+    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
     ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
     IndexFieldTypeDef,
@@ -382,15 +381,15 @@
     DescribeSuggestersResponseTypeDef,
     DefineIndexFieldResponseTypeDef,
     DeleteIndexFieldResponseTypeDef,
     DescribeIndexFieldsResponseTypeDef,
 )
 
 
-def get_structure() -> OptionStatusTypeDef:
+def get_value() -> OptionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/README.md` & `types-aiobotocore-cloudsearch-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudsearch"></a>
 
 # types-aiobotocore-cloudsearch
 
 [![PyPI - types-aiobotocore-cloudsearch](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearch)](https://pepy.tech/project/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [types-aiobotocore-cloudsearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/).
 
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
@@ -254,27 +254,27 @@
 )
 
 
 def check_value(value: AlgorithmicStemmingType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudsearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudsearch.type_defs import (
     OptionStatusTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    BuildSuggestersResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDomainRequestRequestTypeDef,
     DateArrayOptionsTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
@@ -292,30 +292,30 @@
     DocumentSuggesterOptionsTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
     DoubleArrayOptionsTypeDef,
     DoubleOptionsTypeDef,
     IndexDocumentsRequestRequestTypeDef,
-    IndexDocumentsResponseTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
-    ListDomainNamesResponseTypeDef,
-    ResponseMetadataTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
     AnalysisSchemeTypeDef,
+    BuildSuggestersResponseTypeDef,
+    IndexDocumentsResponseTypeDef,
+    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
     ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
     IndexFieldTypeDef,
@@ -349,15 +349,15 @@
     DescribeSuggestersResponseTypeDef,
     DefineIndexFieldResponseTypeDef,
     DeleteIndexFieldResponseTypeDef,
     DescribeIndexFieldsResponseTypeDef,
 )
 
 
-def get_structure() -> OptionStatusTypeDef:
+def get_value() -> OptionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/setup.py` & `types-aiobotocore-cloudsearch-2.5.2.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearch",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudsearch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudsearch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudsearch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/"
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__main__.py` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearch 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudSearch 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.py` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.pyi` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.py` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.pyi` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.py` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudsearch.type_defs import OptionStatusTypeDef
 
-    data: OptionStatusTypeDef = {...}
+    data: OptionStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -31,15 +31,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "OptionStatusTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
-    "BuildSuggestersResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "DateArrayOptionsTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
@@ -57,30 +57,30 @@
     "DocumentSuggesterOptionsTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
     "DoubleArrayOptionsTypeDef",
     "DoubleOptionsTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
-    "IndexDocumentsResponseTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
-    "ListDomainNamesResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
     "AnalysisSchemeTypeDef",
+    "BuildSuggestersResponseTypeDef",
+    "IndexDocumentsResponseTypeDef",
+    "ListDomainNamesResponseTypeDef",
     "DefineExpressionRequestRequestTypeDef",
     "ExpressionStatusTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
     "IndexFieldTypeDef",
@@ -154,19 +154,22 @@
 BuildSuggestersRequestRequestTypeDef = TypedDict(
     "BuildSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-BuildSuggestersResponseTypeDef = TypedDict(
-    "BuildSuggestersResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -493,22 +496,14 @@
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-IndexDocumentsResponseTypeDef = TypedDict(
-    "IndexDocumentsResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -589,33 +584,14 @@
         "SortEnabled": bool,
         "HighlightEnabled": bool,
         "AnalysisScheme": str,
     },
     total=False,
 )
 
-ListDomainNamesResponseTypeDef = TypedDict(
-    "ListDomainNamesResponseTypeDef",
-    {
-        "DomainNames": Dict[str, str],
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
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -670,14 +646,38 @@
 )
 
 
 class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
 
+BuildSuggestersResponseTypeDef = TypedDict(
+    "BuildSuggestersResponseTypeDef",
+    {
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IndexDocumentsResponseTypeDef = TypedDict(
+    "IndexDocumentsResponseTypeDef",
+    {
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainNamesResponseTypeDef = TypedDict(
+    "ListDomainNamesResponseTypeDef",
+    {
+        "DomainNames": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
@@ -790,39 +790,39 @@
     },
 )
 
 DescribeServiceAccessPoliciesResponseTypeDef = TypedDict(
     "DescribeServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceAccessPoliciesResponseTypeDef = TypedDict(
     "UpdateServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAvailabilityOptionsResponseTypeDef = TypedDict(
     "DescribeAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAvailabilityOptionsResponseTypeDef = TypedDict(
     "UpdateAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
         "Options": AnalysisSchemeTypeDef,
@@ -838,31 +838,31 @@
     },
 )
 
 DefineExpressionResponseTypeDef = TypedDict(
     "DefineExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteExpressionResponseTypeDef = TypedDict(
     "DeleteExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExpressionsResponseTypeDef = TypedDict(
     "DescribeExpressionsResponseTypeDef",
     {
         "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -878,47 +878,47 @@
     },
 )
 
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsResponseTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineIndexFieldRequestRequestTypeDef = TypedDict(
     "DefineIndexFieldRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -934,90 +934,90 @@
     },
 )
 
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScalingParametersResponseTypeDef = TypedDict(
     "UpdateScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineAnalysisSchemeResponseTypeDef = TypedDict(
     "DefineAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAnalysisSchemeResponseTypeDef = TypedDict(
     "DeleteAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnalysisSchemesResponseTypeDef = TypedDict(
     "DescribeAnalysisSchemesResponseTypeDef",
     {
         "AnalysisSchemes": List[AnalysisSchemeStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterResponseTypeDef = TypedDict(
     "DefineSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSuggesterResponseTypeDef = TypedDict(
     "DeleteSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSuggestersResponseTypeDef = TypedDict(
     "DescribeSuggestersResponseTypeDef",
     {
         "Suggesters": List[SuggesterStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineIndexFieldResponseTypeDef = TypedDict(
     "DefineIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIndexFieldResponseTypeDef = TypedDict(
     "DeleteIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIndexFieldsResponseTypeDef = TypedDict(
     "DescribeIndexFieldsResponseTypeDef",
     {
         "IndexFields": List[IndexFieldStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.pyi` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudsearch.type_defs import OptionStatusTypeDef
 
-    data: OptionStatusTypeDef = {...}
+    data: OptionStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -30,15 +30,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "OptionStatusTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
-    "BuildSuggestersResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "DateArrayOptionsTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
@@ -56,30 +56,30 @@
     "DocumentSuggesterOptionsTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
     "DoubleArrayOptionsTypeDef",
     "DoubleOptionsTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
-    "IndexDocumentsResponseTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
-    "ListDomainNamesResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
     "AnalysisSchemeTypeDef",
+    "BuildSuggestersResponseTypeDef",
+    "IndexDocumentsResponseTypeDef",
+    "ListDomainNamesResponseTypeDef",
     "DefineExpressionRequestRequestTypeDef",
     "ExpressionStatusTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
     "IndexFieldTypeDef",
@@ -151,19 +151,22 @@
 BuildSuggestersRequestRequestTypeDef = TypedDict(
     "BuildSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-BuildSuggestersResponseTypeDef = TypedDict(
-    "BuildSuggestersResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -474,22 +477,14 @@
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-IndexDocumentsResponseTypeDef = TypedDict(
-    "IndexDocumentsResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -570,33 +565,14 @@
         "SortEnabled": bool,
         "HighlightEnabled": bool,
         "AnalysisScheme": str,
     },
     total=False,
 )
 
-ListDomainNamesResponseTypeDef = TypedDict(
-    "ListDomainNamesResponseTypeDef",
-    {
-        "DomainNames": Dict[str, str],
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
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -649,14 +625,38 @@
     },
     total=False,
 )
 
 class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
+BuildSuggestersResponseTypeDef = TypedDict(
+    "BuildSuggestersResponseTypeDef",
+    {
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IndexDocumentsResponseTypeDef = TypedDict(
+    "IndexDocumentsResponseTypeDef",
+    {
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainNamesResponseTypeDef = TypedDict(
+    "ListDomainNamesResponseTypeDef",
+    {
+        "DomainNames": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
@@ -765,39 +765,39 @@
     },
 )
 
 DescribeServiceAccessPoliciesResponseTypeDef = TypedDict(
     "DescribeServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceAccessPoliciesResponseTypeDef = TypedDict(
     "UpdateServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAvailabilityOptionsResponseTypeDef = TypedDict(
     "DescribeAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAvailabilityOptionsResponseTypeDef = TypedDict(
     "UpdateAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
         "Options": AnalysisSchemeTypeDef,
@@ -813,31 +813,31 @@
     },
 )
 
 DefineExpressionResponseTypeDef = TypedDict(
     "DefineExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteExpressionResponseTypeDef = TypedDict(
     "DeleteExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExpressionsResponseTypeDef = TypedDict(
     "DescribeExpressionsResponseTypeDef",
     {
         "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -853,47 +853,47 @@
     },
 )
 
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsResponseTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineIndexFieldRequestRequestTypeDef = TypedDict(
     "DefineIndexFieldRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -909,90 +909,90 @@
     },
 )
 
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScalingParametersResponseTypeDef = TypedDict(
     "UpdateScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineAnalysisSchemeResponseTypeDef = TypedDict(
     "DefineAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAnalysisSchemeResponseTypeDef = TypedDict(
     "DeleteAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnalysisSchemesResponseTypeDef = TypedDict(
     "DescribeAnalysisSchemesResponseTypeDef",
     {
         "AnalysisSchemes": List[AnalysisSchemeStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterResponseTypeDef = TypedDict(
     "DefineSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSuggesterResponseTypeDef = TypedDict(
     "DeleteSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSuggestersResponseTypeDef = TypedDict(
     "DescribeSuggestersResponseTypeDef",
     {
         "Suggesters": List[SuggesterStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineIndexFieldResponseTypeDef = TypedDict(
     "DefineIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIndexFieldResponseTypeDef = TypedDict(
     "DeleteIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIndexFieldsResponseTypeDef = TypedDict(
     "DescribeIndexFieldsResponseTypeDef",
     {
         "IndexFields": List[IndexFieldStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/PKG-INFO` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudsearch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudsearch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudsearch"></a>
 
 # types-aiobotocore-cloudsearch
 
 [![PyPI - types-aiobotocore-cloudsearch](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearch)](https://pepy.tech/project/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [types-aiobotocore-cloudsearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/).
 
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
@@ -287,27 +286,27 @@
 )
 
 
 def check_value(value: AlgorithmicStemmingType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudsearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudsearch.type_defs import (
     OptionStatusTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    BuildSuggestersResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDomainRequestRequestTypeDef,
     DateArrayOptionsTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
@@ -325,30 +324,30 @@
     DocumentSuggesterOptionsTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
     DoubleArrayOptionsTypeDef,
     DoubleOptionsTypeDef,
     IndexDocumentsRequestRequestTypeDef,
-    IndexDocumentsResponseTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
-    ListDomainNamesResponseTypeDef,
-    ResponseMetadataTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
     AnalysisSchemeTypeDef,
+    BuildSuggestersResponseTypeDef,
+    IndexDocumentsResponseTypeDef,
+    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
     ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
     IndexFieldTypeDef,
@@ -382,15 +381,15 @@
     DescribeSuggestersResponseTypeDef,
     DefineIndexFieldResponseTypeDef,
     DeleteIndexFieldResponseTypeDef,
     DescribeIndexFieldsResponseTypeDef,
 )
 
 
-def get_structure() -> OptionStatusTypeDef:
+def get_value() -> OptionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-translate-2.5.2.tar.gz` & `tmp/types-aiobotocore-translate-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-translate-2.5.2.tar", last modified: Sat Jul  8 01:44:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-translate-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
```

## Comparing `types-aiobotocore-translate-2.5.2.tar` & `types-aiobotocore-translate-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.491017 types-aiobotocore-translate-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-08 01:44:26.491017 types-aiobotocore-translate-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:26.491017 types-aiobotocore-translate-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.491017 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-07-08 01:42:10.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:09.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.491017 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-08 01:44:26.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:44:26.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:26.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:26.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:26.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:44:26.000000 types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-08-02 14:50:46.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-08-02 14:50:46.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-translate-2.5.2/LICENSE` & `types-aiobotocore-translate-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/PKG-INFO` & `types-aiobotocore-translate-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore translate type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore translate type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-translate"></a>
 
 # types-aiobotocore-translate
 
 [![PyPI - types-aiobotocore-translate](https://img.shields.io/pypi/v/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-translate?color=blue)](https://pypistats.org/packages/types-aiobotocore-translate)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Translate 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
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
@@ -317,85 +316,87 @@
 )
 
 
 def check_value(value: DirectionalityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_translate.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_translate.type_defs import (
     TermTypeDef,
+    BlobTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    CreateParallelDataResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
-    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
-    DocumentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
-    TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
-    ListTerminologiesRequestRequestTypeDef,
-    TextTranslationJobFilterTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListTerminologiesRequestRequestTypeDef,
     TranslationSettingsTypeDef,
-    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
-    StopTextTranslationJobResponseTypeDef,
+    TimestampTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
+    DocumentTypeDef,
+    TerminologyDataTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ImportTerminologyRequestRequestTypeDef,
+    CreateParallelDataResponseTypeDef,
+    DeleteParallelDataResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartTextTranslationJobResponseTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    UpdateParallelDataResponseTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTextTranslationJobsRequestRequestTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     TranslateTextRequestRequestTypeDef,
+    TextTranslationJobFilterTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
+    TranslateDocumentRequestRequestTypeDef,
+    ImportTerminologyRequestRequestTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
     ListParallelDataResponseTypeDef,
+    ListTextTranslationJobsRequestRequestTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
     ListTextTranslationJobsResponseTypeDef,
 )
 
 
-def get_structure() -> TermTypeDef:
+def get_value() -> TermTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-translate-2.5.2/README.md` & `types-aiobotocore-translate-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-translate"></a>
 
 # types-aiobotocore-translate
 
 [![PyPI - types-aiobotocore-translate](https://img.shields.io/pypi/v/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-translate?color=blue)](https://pypistats.org/packages/types-aiobotocore-translate)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Translate 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
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
@@ -284,85 +284,87 @@
 )
 
 
 def check_value(value: DirectionalityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_translate.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_translate.type_defs import (
     TermTypeDef,
+    BlobTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    CreateParallelDataResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
-    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
-    DocumentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
-    TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
-    ListTerminologiesRequestRequestTypeDef,
-    TextTranslationJobFilterTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListTerminologiesRequestRequestTypeDef,
     TranslationSettingsTypeDef,
-    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
-    StopTextTranslationJobResponseTypeDef,
+    TimestampTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
+    DocumentTypeDef,
+    TerminologyDataTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ImportTerminologyRequestRequestTypeDef,
+    CreateParallelDataResponseTypeDef,
+    DeleteParallelDataResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartTextTranslationJobResponseTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    UpdateParallelDataResponseTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTextTranslationJobsRequestRequestTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     TranslateTextRequestRequestTypeDef,
+    TextTranslationJobFilterTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
+    TranslateDocumentRequestRequestTypeDef,
+    ImportTerminologyRequestRequestTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
     ListParallelDataResponseTypeDef,
+    ListTextTranslationJobsRequestRequestTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
     ListTextTranslationJobsResponseTypeDef,
 )
 
 
-def get_structure() -> TermTypeDef:
+def get_value() -> TermTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-translate-2.5.2/setup.py` & `types-aiobotocore-translate-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-translate",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore translate type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore translate type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_translate": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/"
```

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/__init__.py` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/__init__.pyi` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/__main__.py` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Translate 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Translate 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
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

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/client.py` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/client.pyi` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/literals.py` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/literals.pyi` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/paginator.py` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListTerminologiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/paginator.pyi` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListTerminologiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/type_defs.py` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_translate.type_defs import TermTypeDef
 
-    data: TermTypeDef = {...}
+    data: TermTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -35,82 +35,85 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TermTypeDef",
+    "BlobTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "CreateParallelDataResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
-    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
-    "DocumentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
-    "TerminologyDataTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    "ListTerminologiesRequestRequestTypeDef",
-    "TextTranslationJobFilterTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListTerminologiesRequestRequestTypeDef",
     "TranslationSettingsTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
+    "TimestampTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
+    "DocumentTypeDef",
+    "TerminologyDataTypeDef",
     "OutputDataConfigTypeDef",
     "TerminologyPropertiesTypeDef",
     "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ImportTerminologyRequestRequestTypeDef",
+    "CreateParallelDataResponseTypeDef",
+    "DeleteParallelDataResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "ListLanguagesResponseTypeDef",
-    "ListTextTranslationJobsRequestRequestTypeDef",
-    "TranslateDocumentRequestRequestTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "TranslateTextRequestRequestTypeDef",
+    "TextTranslationJobFilterTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
+    "TranslateDocumentRequestRequestTypeDef",
+    "ImportTerminologyRequestRequestTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
     "ImportTerminologyResponseTypeDef",
     "ListTerminologiesResponseTypeDef",
     "GetParallelDataResponseTypeDef",
     "ListParallelDataResponseTypeDef",
+    "ListTextTranslationJobsRequestRequestTypeDef",
     "DescribeTextTranslationJobResponseTypeDef",
     "ListTextTranslationJobsResponseTypeDef",
 )
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
     },
 )
@@ -127,68 +130,46 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeTextTranslationJobRequestRequestTypeDef = TypedDict(
     "DescribeTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DocumentTypeDef = TypedDict(
-    "DocumentTypeDef",
-    {
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -225,34 +206,14 @@
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
 
-_RequiredTerminologyDataTypeDef = TypedDict(
-    "_RequiredTerminologyDataTypeDef",
-    {
-        "File": Union[str, bytes, IO[Any], StreamingBody],
-        "Format": TerminologyDataFormatType,
-    },
-)
-_OptionalTerminologyDataTypeDef = TypedDict(
-    "_OptionalTerminologyDataTypeDef",
-    {
-        "Directionality": DirectionalityType,
-    },
-    total=False,
-)
-
-
-class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
-    pass
-
-
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -297,97 +258,50 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListTerminologiesRequestRequestTypeDef = TypedDict(
-    "ListTerminologiesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-TextTranslationJobFilterTypeDef = TypedDict(
-    "TextTranslationJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBeforeTime": Union[datetime, str],
-        "SubmittedAfterTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListTerminologiesRequestRequestTypeDef = TypedDict(
+    "ListTerminologiesRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
 
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
 )
 
@@ -395,34 +309,51 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
+AppliedTerminologyTypeDef = TypedDict(
+    "AppliedTerminologyTypeDef",
     {
         "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Terms": List[TermTypeDef],
     },
+    total=False,
 )
 
-AppliedTerminologyTypeDef = TypedDict(
-    "AppliedTerminologyTypeDef",
+DocumentTypeDef = TypedDict(
+    "DocumentTypeDef",
     {
-        "Name": str,
-        "Terms": List[TermTypeDef],
+        "Content": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+
+_RequiredTerminologyDataTypeDef = TypedDict(
+    "_RequiredTerminologyDataTypeDef",
+    {
+        "File": BlobTypeDef,
+        "Format": TerminologyDataFormatType,
+    },
+)
+_OptionalTerminologyDataTypeDef = TypedDict(
+    "_OptionalTerminologyDataTypeDef",
+    {
+        "Directionality": DirectionalityType,
     },
     total=False,
 )
 
+
+class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
+    pass
+
+
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
@@ -529,99 +460,102 @@
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
-    "_RequiredImportTerminologyRequestRequestTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
         "Name": str,
-        "MergeStrategy": Literal["OVERWRITE"],
-        "TerminologyData": TerminologyDataTypeDef,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalImportTerminologyRequestRequestTypeDef = TypedDict(
-    "_OptionalImportTerminologyRequestRequestTypeDef",
+
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
     {
-        "Description": str,
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "Tags": Sequence[TagTypeDef],
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ImportTerminologyRequestRequestTypeDef(
-    _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
-):
-    pass
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListLanguagesResponseTypeDef = TypedDict(
-    "ListLanguagesResponseTypeDef",
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
     {
-        "Languages": List[LanguageTypeDef],
-        "DisplayLanguageCode": DisplayLanguageCodeType,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
-    "ListTextTranslationJobsRequestRequestTypeDef",
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
     {
-        "Filter": TextTranslationJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredTranslateDocumentRequestRequestTypeDef",
+ListLanguagesResponseTypeDef = TypedDict(
+    "ListLanguagesResponseTypeDef",
     {
-        "Document": DocumentTypeDef,
-        "SourceLanguageCode": str,
-        "TargetLanguageCode": str,
+        "Languages": List[LanguageTypeDef],
+        "DisplayLanguageCode": DisplayLanguageCodeType,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalTranslateDocumentRequestRequestTypeDef",
+
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
-        "TerminologyNames": Sequence[str],
-        "Settings": TranslationSettingsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class TranslateDocumentRequestRequestTypeDef(
-    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -638,37 +572,97 @@
 
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
 
+TextTranslationJobFilterTypeDef = TypedDict(
+    "TextTranslationJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBeforeTime": TimestampTypeDef,
+        "SubmittedAfterTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredTranslateDocumentRequestRequestTypeDef",
+    {
+        "Document": DocumentTypeDef,
+        "SourceLanguageCode": str,
+        "TargetLanguageCode": str,
+    },
+)
+_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalTranslateDocumentRequestRequestTypeDef",
+    {
+        "TerminologyNames": Sequence[str],
+        "Settings": TranslationSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class TranslateDocumentRequestRequestTypeDef(
+    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
+    "_RequiredImportTerminologyRequestRequestTypeDef",
+    {
+        "Name": str,
+        "MergeStrategy": Literal["OVERWRITE"],
+        "TerminologyData": TerminologyDataTypeDef,
     },
 )
+_OptionalImportTerminologyRequestRequestTypeDef = TypedDict(
+    "_OptionalImportTerminologyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "EncryptionKey": EncryptionKeyTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportTerminologyRequestRequestTypeDef(
+    _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
@@ -720,65 +714,75 @@
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
+    "ListTextTranslationJobsRequestRequestTypeDef",
+    {
+        "Filter": TextTranslationJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate/type_defs.pyi` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_translate.type_defs import TermTypeDef
 
-    data: TermTypeDef = {...}
+    data: TermTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -34,82 +34,85 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TermTypeDef",
+    "BlobTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "CreateParallelDataResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
-    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
-    "DocumentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
-    "TerminologyDataTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    "ListTerminologiesRequestRequestTypeDef",
-    "TextTranslationJobFilterTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListTerminologiesRequestRequestTypeDef",
     "TranslationSettingsTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
+    "TimestampTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
+    "DocumentTypeDef",
+    "TerminologyDataTypeDef",
     "OutputDataConfigTypeDef",
     "TerminologyPropertiesTypeDef",
     "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ImportTerminologyRequestRequestTypeDef",
+    "CreateParallelDataResponseTypeDef",
+    "DeleteParallelDataResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "ListLanguagesResponseTypeDef",
-    "ListTextTranslationJobsRequestRequestTypeDef",
-    "TranslateDocumentRequestRequestTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "TranslateTextRequestRequestTypeDef",
+    "TextTranslationJobFilterTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
+    "TranslateDocumentRequestRequestTypeDef",
+    "ImportTerminologyRequestRequestTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
     "ImportTerminologyResponseTypeDef",
     "ListTerminologiesResponseTypeDef",
     "GetParallelDataResponseTypeDef",
     "ListParallelDataResponseTypeDef",
+    "ListTextTranslationJobsRequestRequestTypeDef",
     "DescribeTextTranslationJobResponseTypeDef",
     "ListTextTranslationJobsResponseTypeDef",
 )
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
     },
 )
@@ -126,68 +129,46 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeTextTranslationJobRequestRequestTypeDef = TypedDict(
     "DescribeTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DocumentTypeDef = TypedDict(
-    "DocumentTypeDef",
-    {
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -222,32 +203,14 @@
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
 
-_RequiredTerminologyDataTypeDef = TypedDict(
-    "_RequiredTerminologyDataTypeDef",
-    {
-        "File": Union[str, bytes, IO[Any], StreamingBody],
-        "Format": TerminologyDataFormatType,
-    },
-)
-_OptionalTerminologyDataTypeDef = TypedDict(
-    "_OptionalTerminologyDataTypeDef",
-    {
-        "Directionality": DirectionalityType,
-    },
-    total=False,
-)
-
-class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
-    pass
-
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -292,97 +255,50 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListTerminologiesRequestRequestTypeDef = TypedDict(
-    "ListTerminologiesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-TextTranslationJobFilterTypeDef = TypedDict(
-    "TextTranslationJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBeforeTime": Union[datetime, str],
-        "SubmittedAfterTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListTerminologiesRequestRequestTypeDef = TypedDict(
+    "ListTerminologiesRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
 
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
 )
 
@@ -390,34 +306,49 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
+AppliedTerminologyTypeDef = TypedDict(
+    "AppliedTerminologyTypeDef",
     {
         "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Terms": List[TermTypeDef],
     },
+    total=False,
 )
 
-AppliedTerminologyTypeDef = TypedDict(
-    "AppliedTerminologyTypeDef",
+DocumentTypeDef = TypedDict(
+    "DocumentTypeDef",
     {
-        "Name": str,
-        "Terms": List[TermTypeDef],
+        "Content": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+
+_RequiredTerminologyDataTypeDef = TypedDict(
+    "_RequiredTerminologyDataTypeDef",
+    {
+        "File": BlobTypeDef,
+        "Format": TerminologyDataFormatType,
+    },
+)
+_OptionalTerminologyDataTypeDef = TypedDict(
+    "_OptionalTerminologyDataTypeDef",
+    {
+        "Directionality": DirectionalityType,
     },
     total=False,
 )
 
+class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
+    pass
+
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
@@ -518,94 +449,101 @@
 
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
-    "_RequiredImportTerminologyRequestRequestTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
         "Name": str,
-        "MergeStrategy": Literal["OVERWRITE"],
-        "TerminologyData": TerminologyDataTypeDef,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalImportTerminologyRequestRequestTypeDef = TypedDict(
-    "_OptionalImportTerminologyRequestRequestTypeDef",
+
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
     {
-        "Description": str,
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "Tags": Sequence[TagTypeDef],
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ImportTerminologyRequestRequestTypeDef(
-    _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
-):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListLanguagesResponseTypeDef = TypedDict(
-    "ListLanguagesResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Languages": List[LanguageTypeDef],
-        "DisplayLanguageCode": DisplayLanguageCodeType,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
-    "ListTextTranslationJobsRequestRequestTypeDef",
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
     {
-        "Filter": TextTranslationJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredTranslateDocumentRequestRequestTypeDef",
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
     {
-        "Document": DocumentTypeDef,
-        "SourceLanguageCode": str,
-        "TargetLanguageCode": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalTranslateDocumentRequestRequestTypeDef",
+
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
     {
-        "TerminologyNames": Sequence[str],
-        "Settings": TranslationSettingsTypeDef,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class TranslateDocumentRequestRequestTypeDef(
-    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
-):
-    pass
+ListLanguagesResponseTypeDef = TypedDict(
+    "ListLanguagesResponseTypeDef",
+    {
+        "Languages": List[LanguageTypeDef],
+        "DisplayLanguageCode": DisplayLanguageCodeType,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
@@ -621,38 +559,94 @@
 )
 
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
+TextTranslationJobFilterTypeDef = TypedDict(
+    "TextTranslationJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBeforeTime": TimestampTypeDef,
+        "SubmittedAfterTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredTranslateDocumentRequestRequestTypeDef",
+    {
+        "Document": DocumentTypeDef,
+        "SourceLanguageCode": str,
+        "TargetLanguageCode": str,
+    },
+)
+_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalTranslateDocumentRequestRequestTypeDef",
+    {
+        "TerminologyNames": Sequence[str],
+        "Settings": TranslationSettingsTypeDef,
+    },
+    total=False,
+)
+
+class TranslateDocumentRequestRequestTypeDef(
+    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
+):
+    pass
+
+_RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
+    "_RequiredImportTerminologyRequestRequestTypeDef",
+    {
+        "Name": str,
+        "MergeStrategy": Literal["OVERWRITE"],
+        "TerminologyData": TerminologyDataTypeDef,
+    },
+)
+_OptionalImportTerminologyRequestRequestTypeDef = TypedDict(
+    "_OptionalImportTerminologyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "EncryptionKey": EncryptionKeyTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+class ImportTerminologyRequestRequestTypeDef(
+    _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
+):
+    pass
+
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "SourceLanguageCode": str,
@@ -701,65 +695,75 @@
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
+    "ListTextTranslationJobsRequestRequestTypeDef",
+    {
+        "Filter": TextTranslationJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/PKG-INFO` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore translate type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore translate type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-translate"></a>
 
 # types-aiobotocore-translate
 
 [![PyPI - types-aiobotocore-translate](https://img.shields.io/pypi/v/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-translate?color=blue)](https://pypistats.org/packages/types-aiobotocore-translate)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Translate 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
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
@@ -317,85 +316,87 @@
 )
 
 
 def check_value(value: DirectionalityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_translate.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_translate.type_defs import (
     TermTypeDef,
+    BlobTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    CreateParallelDataResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
-    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
-    DocumentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
-    TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
-    ListTerminologiesRequestRequestTypeDef,
-    TextTranslationJobFilterTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListTerminologiesRequestRequestTypeDef,
     TranslationSettingsTypeDef,
-    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
-    StopTextTranslationJobResponseTypeDef,
+    TimestampTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
+    DocumentTypeDef,
+    TerminologyDataTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ImportTerminologyRequestRequestTypeDef,
+    CreateParallelDataResponseTypeDef,
+    DeleteParallelDataResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartTextTranslationJobResponseTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    UpdateParallelDataResponseTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTextTranslationJobsRequestRequestTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     TranslateTextRequestRequestTypeDef,
+    TextTranslationJobFilterTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
+    TranslateDocumentRequestRequestTypeDef,
+    ImportTerminologyRequestRequestTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
     ListParallelDataResponseTypeDef,
+    ListTextTranslationJobsRequestRequestTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
     ListTextTranslationJobsResponseTypeDef,
 )
 
 
-def get_structure() -> TermTypeDef:
+def get_value() -> TermTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-translate-2.5.2/types_aiobotocore_translate.egg-info/SOURCES.txt` & `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*


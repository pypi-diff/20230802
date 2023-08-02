# Comparing `tmp/types-aiobotocore-cloudsearchdomain-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudsearchdomain-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearchdomain-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearchdomain-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
```

## Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.tar` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.673828 types-aiobotocore-cloudsearchdomain-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-08 01:43:21.669828 types-aiobotocore-cloudsearchdomain-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.673828 types-aiobotocore-cloudsearchdomain-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.669828 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-08 01:27:12.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-08 01:27:12.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-08 01:27:12.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.669828 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.281636 types-aiobotocore-cloudsearchdomain-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-02 14:52:00.273636 types-aiobotocore-cloudsearchdomain-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.281636 types-aiobotocore-cloudsearchdomain-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.269636 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-08-02 14:34:44.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-02 14:34:44.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.273636 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/LICENSE` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/PKG-INFO` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearchdomain
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudsearchdomain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudsearchdomain type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudsearchdomain"></a>
 
 # types-aiobotocore-cloudsearchdomain
 
 [![PyPI - types-aiobotocore-cloudsearchdomain](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearchdomain?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearchdomain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudSearchDomain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [types-aiobotocore-cloudsearchdomain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/).
 
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
@@ -281,44 +280,45 @@
 )
 
 
 def check_value(value: ContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudsearchdomain.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudsearchdomain.type_defs import (
+    BlobTypeDef,
     BucketTypeDef,
     DocumentServiceWarningTypeDef,
     FieldStatsTypeDef,
     HitTypeDef,
     ResponseMetadataTypeDef,
     SearchRequestRequestTypeDef,
     SearchStatusTypeDef,
     SuggestionMatchTypeDef,
     SuggestRequestRequestTypeDef,
     SuggestStatusTypeDef,
     UploadDocumentsRequestRequestTypeDef,
     BucketInfoTypeDef,
-    UploadDocumentsResponseTypeDef,
     HitsTypeDef,
+    UploadDocumentsResponseTypeDef,
     SuggestModelTypeDef,
     SearchResponseTypeDef,
     SuggestResponseTypeDef,
 )
 
 
-def get_structure() -> BucketTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/README.md` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudsearchdomain"></a>
 
 # types-aiobotocore-cloudsearchdomain
 
 [![PyPI - types-aiobotocore-cloudsearchdomain](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearchdomain?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearchdomain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudSearchDomain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [types-aiobotocore-cloudsearchdomain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/).
 
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
@@ -248,44 +248,45 @@
 )
 
 
 def check_value(value: ContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudsearchdomain.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudsearchdomain.type_defs import (
+    BlobTypeDef,
     BucketTypeDef,
     DocumentServiceWarningTypeDef,
     FieldStatsTypeDef,
     HitTypeDef,
     ResponseMetadataTypeDef,
     SearchRequestRequestTypeDef,
     SearchStatusTypeDef,
     SuggestionMatchTypeDef,
     SuggestRequestRequestTypeDef,
     SuggestStatusTypeDef,
     UploadDocumentsRequestRequestTypeDef,
     BucketInfoTypeDef,
-    UploadDocumentsResponseTypeDef,
     HitsTypeDef,
+    UploadDocumentsResponseTypeDef,
     SuggestModelTypeDef,
     SearchResponseTypeDef,
     SuggestResponseTypeDef,
 )
 
 
-def get_structure() -> BucketTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/setup.py` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearchdomain",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudsearchdomain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with"
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
-        "aiobotocore cloudsearchdomain type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore cloudsearchdomain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudsearchdomain": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/"
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/__init__.py` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/__init__.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/__main__.py` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearchDomain 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudSearchDomain 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain\nOther"
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

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/client.py` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,40 +10,41 @@
     from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient
 
     session = get_session()
     async with session.create_client("cloudsearchdomain") as client:
         client: CloudSearchDomainClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import ContentTypeType, QueryParserType
-from .type_defs import SearchResponseTypeDef, SuggestResponseTypeDef, UploadDocumentsResponseTypeDef
+from .type_defs import (
+    BlobTypeDef,
+    SearchResponseTypeDef,
+    SuggestResponseTypeDef,
+    UploadDocumentsResponseTypeDef,
+)
 
 __all__ = ("CloudSearchDomainClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DocumentServiceException: Type[BotocoreClientError]
     SearchException: Type[BotocoreClientError]
 
-
 class CloudSearchDomainClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/)
     """
 
     meta: ClientMeta
@@ -52,45 +53,41 @@
     def exceptions(self) -> Exceptions:
         """
         CloudSearchDomainClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#close)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#generate_presigned_url)
         """
-
     async def search(
         self,
         *,
         query: str,
         cursor: str = ...,
         expr: str = ...,
         facet: str = ...,
@@ -107,39 +104,35 @@
     ) -> SearchResponseTypeDef:
         """
         Retrieves a list of documents that match the specified search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#search)
         """
-
     async def suggest(
         self, *, query: str, suggester: str, size: int = ...
     ) -> SuggestResponseTypeDef:
         """
         Retrieves autocomplete suggestions for a partial query string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.suggest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#suggest)
         """
-
     async def upload_documents(
-        self, *, documents: Union[str, bytes, IO[Any], StreamingBody], contentType: ContentTypeType
+        self, *, documents: BlobTypeDef, contentType: ContentTypeType
     ) -> UploadDocumentsResponseTypeDef:
         """
         Posts a batch of documents to a search domain for indexing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.upload_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#upload_documents)
         """
-
     async def __aenter__(self) -> "CloudSearchDomainClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/)
         """
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/client.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,44 @@
     from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient
 
     session = get_session()
     async with session.create_client("cloudsearchdomain") as client:
         client: CloudSearchDomainClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import ContentTypeType, QueryParserType
-from .type_defs import SearchResponseTypeDef, SuggestResponseTypeDef, UploadDocumentsResponseTypeDef
+from .type_defs import (
+    BlobTypeDef,
+    SearchResponseTypeDef,
+    SuggestResponseTypeDef,
+    UploadDocumentsResponseTypeDef,
+)
 
 __all__ = ("CloudSearchDomainClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DocumentServiceException: Type[BotocoreClientError]
     SearchException: Type[BotocoreClientError]
 
+
 class CloudSearchDomainClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/)
     """
 
     meta: ClientMeta
@@ -49,41 +56,45 @@
     def exceptions(self) -> Exceptions:
         """
         CloudSearchDomainClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#close)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#generate_presigned_url)
         """
+
     async def search(
         self,
         *,
         query: str,
         cursor: str = ...,
         expr: str = ...,
         facet: str = ...,
@@ -100,35 +111,39 @@
     ) -> SearchResponseTypeDef:
         """
         Retrieves a list of documents that match the specified search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#search)
         """
+
     async def suggest(
         self, *, query: str, suggester: str, size: int = ...
     ) -> SuggestResponseTypeDef:
         """
         Retrieves autocomplete suggestions for a partial query string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.suggest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#suggest)
         """
+
     async def upload_documents(
-        self, *, documents: Union[str, bytes, IO[Any], StreamingBody], contentType: ContentTypeType
+        self, *, documents: BlobTypeDef, contentType: ContentTypeType
     ) -> UploadDocumentsResponseTypeDef:
         """
         Posts a batch of documents to a search domain for indexing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.upload_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#upload_documents)
         """
+
     async def __aenter__(self) -> "CloudSearchDomainClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/)
         """
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/literals.py` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/literals.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/type_defs.py` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,52 +2,53 @@
 Type annotations for cloudsearchdomain service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_cloudsearchdomain.type_defs import BucketTypeDef
+    from types_aiobotocore_cloudsearchdomain.type_defs import BlobTypeDef
 
-    data: BucketTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import ContentTypeType, QueryParserType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "BlobTypeDef",
     "BucketTypeDef",
     "DocumentServiceWarningTypeDef",
     "FieldStatsTypeDef",
     "HitTypeDef",
     "ResponseMetadataTypeDef",
     "SearchRequestRequestTypeDef",
     "SearchStatusTypeDef",
     "SuggestionMatchTypeDef",
     "SuggestRequestRequestTypeDef",
     "SuggestStatusTypeDef",
     "UploadDocumentsRequestRequestTypeDef",
     "BucketInfoTypeDef",
-    "UploadDocumentsResponseTypeDef",
     "HitsTypeDef",
+    "UploadDocumentsResponseTypeDef",
     "SuggestModelTypeDef",
     "SearchResponseTypeDef",
     "SuggestResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "value": str,
         "count": int,
     },
     total=False,
@@ -120,21 +121,19 @@
         "sort": str,
         "start": int,
         "stats": str,
     },
     total=False,
 )
 
-
 class SearchRequestRequestTypeDef(
     _RequiredSearchRequestRequestTypeDef, _OptionalSearchRequestRequestTypeDef
 ):
     pass
 
-
 SearchStatusTypeDef = TypedDict(
     "SearchStatusTypeDef",
     {
         "timems": int,
         "rid": str,
     },
     total=False,
@@ -161,68 +160,66 @@
     "_OptionalSuggestRequestRequestTypeDef",
     {
         "size": int,
     },
     total=False,
 )
 
-
 class SuggestRequestRequestTypeDef(
     _RequiredSuggestRequestRequestTypeDef, _OptionalSuggestRequestRequestTypeDef
 ):
     pass
 
-
 SuggestStatusTypeDef = TypedDict(
     "SuggestStatusTypeDef",
     {
         "timems": int,
         "rid": str,
     },
     total=False,
 )
 
 UploadDocumentsRequestRequestTypeDef = TypedDict(
     "UploadDocumentsRequestRequestTypeDef",
     {
-        "documents": Union[str, bytes, IO[Any], StreamingBody],
+        "documents": BlobTypeDef,
         "contentType": ContentTypeType,
     },
 )
 
 BucketInfoTypeDef = TypedDict(
     "BucketInfoTypeDef",
     {
         "buckets": List[BucketTypeDef],
     },
     total=False,
 )
 
-UploadDocumentsResponseTypeDef = TypedDict(
-    "UploadDocumentsResponseTypeDef",
-    {
-        "status": str,
-        "adds": int,
-        "deletes": int,
-        "warnings": List[DocumentServiceWarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HitsTypeDef = TypedDict(
     "HitsTypeDef",
     {
         "found": int,
         "start": int,
         "cursor": str,
         "hit": List[HitTypeDef],
     },
     total=False,
 )
 
+UploadDocumentsResponseTypeDef = TypedDict(
+    "UploadDocumentsResponseTypeDef",
+    {
+        "status": str,
+        "adds": int,
+        "deletes": int,
+        "warnings": List[DocumentServiceWarningTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SuggestModelTypeDef = TypedDict(
     "SuggestModelTypeDef",
     {
         "query": str,
         "found": int,
         "suggestions": List[SuggestionMatchTypeDef],
     },
@@ -232,19 +229,19 @@
 SearchResponseTypeDef = TypedDict(
     "SearchResponseTypeDef",
     {
         "status": SearchStatusTypeDef,
         "hits": HitsTypeDef,
         "facets": Dict[str, BucketInfoTypeDef],
         "stats": Dict[str, FieldStatsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SuggestResponseTypeDef = TypedDict(
     "SuggestResponseTypeDef",
     {
         "status": SuggestStatusTypeDef,
         "suggest": SuggestModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain/type_defs.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,51 +2,54 @@
 Type annotations for cloudsearchdomain service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_cloudsearchdomain.type_defs import BucketTypeDef
+    from types_aiobotocore_cloudsearchdomain.type_defs import BlobTypeDef
 
-    data: BucketTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import ContentTypeType, QueryParserType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "BlobTypeDef",
     "BucketTypeDef",
     "DocumentServiceWarningTypeDef",
     "FieldStatsTypeDef",
     "HitTypeDef",
     "ResponseMetadataTypeDef",
     "SearchRequestRequestTypeDef",
     "SearchStatusTypeDef",
     "SuggestionMatchTypeDef",
     "SuggestRequestRequestTypeDef",
     "SuggestStatusTypeDef",
     "UploadDocumentsRequestRequestTypeDef",
     "BucketInfoTypeDef",
-    "UploadDocumentsResponseTypeDef",
     "HitsTypeDef",
+    "UploadDocumentsResponseTypeDef",
     "SuggestModelTypeDef",
     "SearchResponseTypeDef",
     "SuggestResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "value": str,
         "count": int,
     },
     total=False,
@@ -119,19 +122,21 @@
         "sort": str,
         "start": int,
         "stats": str,
     },
     total=False,
 )
 
+
 class SearchRequestRequestTypeDef(
     _RequiredSearchRequestRequestTypeDef, _OptionalSearchRequestRequestTypeDef
 ):
     pass
 
+
 SearchStatusTypeDef = TypedDict(
     "SearchStatusTypeDef",
     {
         "timems": int,
         "rid": str,
     },
     total=False,
@@ -158,66 +163,68 @@
     "_OptionalSuggestRequestRequestTypeDef",
     {
         "size": int,
     },
     total=False,
 )
 
+
 class SuggestRequestRequestTypeDef(
     _RequiredSuggestRequestRequestTypeDef, _OptionalSuggestRequestRequestTypeDef
 ):
     pass
 
+
 SuggestStatusTypeDef = TypedDict(
     "SuggestStatusTypeDef",
     {
         "timems": int,
         "rid": str,
     },
     total=False,
 )
 
 UploadDocumentsRequestRequestTypeDef = TypedDict(
     "UploadDocumentsRequestRequestTypeDef",
     {
-        "documents": Union[str, bytes, IO[Any], StreamingBody],
+        "documents": BlobTypeDef,
         "contentType": ContentTypeType,
     },
 )
 
 BucketInfoTypeDef = TypedDict(
     "BucketInfoTypeDef",
     {
         "buckets": List[BucketTypeDef],
     },
     total=False,
 )
 
-UploadDocumentsResponseTypeDef = TypedDict(
-    "UploadDocumentsResponseTypeDef",
-    {
-        "status": str,
-        "adds": int,
-        "deletes": int,
-        "warnings": List[DocumentServiceWarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HitsTypeDef = TypedDict(
     "HitsTypeDef",
     {
         "found": int,
         "start": int,
         "cursor": str,
         "hit": List[HitTypeDef],
     },
     total=False,
 )
 
+UploadDocumentsResponseTypeDef = TypedDict(
+    "UploadDocumentsResponseTypeDef",
+    {
+        "status": str,
+        "adds": int,
+        "deletes": int,
+        "warnings": List[DocumentServiceWarningTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SuggestModelTypeDef = TypedDict(
     "SuggestModelTypeDef",
     {
         "query": str,
         "found": int,
         "suggestions": List[SuggestionMatchTypeDef],
     },
@@ -227,19 +234,19 @@
 SearchResponseTypeDef = TypedDict(
     "SearchResponseTypeDef",
     {
         "status": SearchStatusTypeDef,
         "hits": HitsTypeDef,
         "facets": Dict[str, BucketInfoTypeDef],
         "stats": Dict[str, FieldStatsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SuggestResponseTypeDef = TypedDict(
     "SuggestResponseTypeDef",
     {
         "status": SuggestStatusTypeDef,
         "suggest": SuggestModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearchdomain
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudsearchdomain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudsearchdomain type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudsearchdomain"></a>
 
 # types-aiobotocore-cloudsearchdomain
 
 [![PyPI - types-aiobotocore-cloudsearchdomain](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearchdomain?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearchdomain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudSearchDomain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [types-aiobotocore-cloudsearchdomain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/).
 
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
@@ -281,44 +280,45 @@
 )
 
 
 def check_value(value: ContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudsearchdomain.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudsearchdomain.type_defs import (
+    BlobTypeDef,
     BucketTypeDef,
     DocumentServiceWarningTypeDef,
     FieldStatsTypeDef,
     HitTypeDef,
     ResponseMetadataTypeDef,
     SearchRequestRequestTypeDef,
     SearchStatusTypeDef,
     SuggestionMatchTypeDef,
     SuggestRequestRequestTypeDef,
     SuggestStatusTypeDef,
     UploadDocumentsRequestRequestTypeDef,
     BucketInfoTypeDef,
-    UploadDocumentsResponseTypeDef,
     HitsTypeDef,
+    UploadDocumentsResponseTypeDef,
     SuggestModelTypeDef,
     SearchResponseTypeDef,
     SuggestResponseTypeDef,
 )
 
 
-def get_structure() -> BucketTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearchdomain-2.5.2.post1/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*


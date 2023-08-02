# Comparing `tmp/types-aiobotocore-importexport-2.5.2.tar.gz` & `tmp/types-aiobotocore-importexport-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-importexport-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-importexport-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-importexport-2.5.2.tar` & `types-aiobotocore-importexport-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.306257 types-aiobotocore-importexport-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-08 01:43:44.306257 types-aiobotocore-importexport-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.306257 types-aiobotocore-importexport-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:32:12.000000 types-aiobotocore-importexport-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.302257 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:13.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.306257 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-08 01:43:44.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:44.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:44.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:44.000000 types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.125570 types-aiobotocore-importexport-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-08-02 14:52:24.125570 types-aiobotocore-importexport-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.125570 types-aiobotocore-importexport-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.121570 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-02 14:40:13.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:12.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.125570 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-08-02 14:52:23.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:23.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:23.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:23.000000 types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-importexport-2.5.2/LICENSE` & `types-aiobotocore-importexport-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/PKG-INFO` & `types-aiobotocore-importexport-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-importexport
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ImportExport 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ImportExport 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore importexport type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore importexport type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-importexport"></a>
 
 # types-aiobotocore-importexport
 
 [![PyPI - types-aiobotocore-importexport](https://img.shields.io/pypi/v/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-importexport?color=blue)](https://pypistats.org/packages/types-aiobotocore-importexport)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-importexport)](https://pepy.tech/project/types-aiobotocore-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ImportExport 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [types-aiobotocore-importexport docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/).
 
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
@@ -305,44 +304,44 @@
 )
 
 
 def check_value(value: JobTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_importexport.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListJobsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListJobsInputRequestTypeDef,
     UpdateJobInputRequestTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
-def get_structure() -> ArtifactTypeDef:
+def get_value() -> ArtifactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-importexport-2.5.2/README.md` & `types-aiobotocore-importexport-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-importexport"></a>
 
 # types-aiobotocore-importexport
 
 [![PyPI - types-aiobotocore-importexport](https://img.shields.io/pypi/v/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-importexport?color=blue)](https://pypistats.org/packages/types-aiobotocore-importexport)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-importexport)](https://pepy.tech/project/types-aiobotocore-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ImportExport 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [types-aiobotocore-importexport docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/).
 
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
@@ -272,44 +272,44 @@
 )
 
 
 def check_value(value: JobTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_importexport.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListJobsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListJobsInputRequestTypeDef,
     UpdateJobInputRequestTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
-def get_structure() -> ArtifactTypeDef:
+def get_value() -> ArtifactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-importexport-2.5.2/setup.py` & `types-aiobotocore-importexport-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-importexport",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_importexport"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ImportExport 2.5.2 service generated with"
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
-    keywords="aiobotocore importexport type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore importexport type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_importexport": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/"
```

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/__init__.py` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/__init__.pyi` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/__main__.py` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ImportExport 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ImportExport 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport\nOther"
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

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/client.py` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/client.pyi` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/literals.py` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/literals.pyi` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/paginator.py` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, APIVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, APIVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/paginators/#listjobspaginator)
         """
```

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/paginator.pyi` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, APIVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, APIVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/paginators/#listjobspaginator)
         """
```

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/type_defs.py` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_importexport.type_defs import ArtifactTypeDef
 
-    data: ArtifactTypeDef = {...}
+    data: ArtifactTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import JobTypeType
@@ -22,29 +22,29 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
-    "CancelJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
-    "GetShippingLabelOutputTypeDef",
     "GetStatusInputRequestTypeDef",
     "JobTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
-    "ListJobsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListJobsInputRequestTypeDef",
     "UpdateJobInputRequestTypeDef",
+    "CancelJobOutputTypeDef",
     "CreateJobOutputTypeDef",
+    "GetShippingLabelOutputTypeDef",
     "GetStatusOutputTypeDef",
     "UpdateJobOutputTypeDef",
     "ListJobsOutputTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
 )
 
 ArtifactTypeDef = TypedDict(
     "ArtifactTypeDef",
     {
         "Description": str,
         "URL": str,
@@ -69,19 +69,22 @@
 
 class CancelJobInputRequestTypeDef(
     _RequiredCancelJobInputRequestTypeDef, _OptionalCancelJobInputRequestTypeDef
 ):
     pass
 
 
-CancelJobOutputTypeDef = TypedDict(
-    "CancelJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateJobInputRequestTypeDef = TypedDict(
     "_RequiredCreateJobInputRequestTypeDef",
     {
         "JobType": JobTypeType,
@@ -132,23 +135,14 @@
 
 class GetShippingLabelInputRequestTypeDef(
     _RequiredGetShippingLabelInputRequestTypeDef, _OptionalGetShippingLabelInputRequestTypeDef
 ):
     pass
 
 
-GetShippingLabelOutputTypeDef = TypedDict(
-    "GetShippingLabelOutputTypeDef",
-    {
-        "ShippingLabelURL": str,
-        "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatusInputRequestTypeDef = TypedDict(
     "_RequiredGetStatusInputRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetStatusInputRequestTypeDef = TypedDict(
@@ -173,54 +167,34 @@
         "CreationDate": datetime,
         "IsCanceled": bool,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-ListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "ListJobsInputListJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "APIVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListJobsInputRequestTypeDef = TypedDict(
     "ListJobsInputRequestTypeDef",
     {
         "MaxJobs": int,
         "Marker": str,
         "APIVersion": str,
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
 _RequiredUpdateJobInputRequestTypeDef = TypedDict(
     "_RequiredUpdateJobInputRequestTypeDef",
     {
         "JobId": str,
         "Manifest": str,
         "JobType": JobTypeType,
         "ValidateOnly": bool,
@@ -237,24 +211,41 @@
 
 class UpdateJobInputRequestTypeDef(
     _RequiredUpdateJobInputRequestTypeDef, _OptionalUpdateJobInputRequestTypeDef
 ):
     pass
 
 
+CancelJobOutputTypeDef = TypedDict(
+    "CancelJobOutputTypeDef",
+    {
+        "Success": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "JobId": str,
         "JobType": JobTypeType,
         "Signature": str,
         "SignatureFileContents": str,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetShippingLabelOutputTypeDef = TypedDict(
+    "GetShippingLabelOutputTypeDef",
+    {
+        "ShippingLabelURL": str,
+        "Warning": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatusOutputTypeDef = TypedDict(
     "GetStatusOutputTypeDef",
     {
         "JobId": str,
@@ -269,29 +260,38 @@
         "LogKey": str,
         "ErrorCount": int,
         "Signature": str,
         "SignatureFileContents": str,
         "CurrentManifest": str,
         "CreationDate": datetime,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobOutputTypeDef = TypedDict(
     "UpdateJobOutputTypeDef",
     {
         "Success": bool,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "IsTruncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "ListJobsInputListJobsPaginateTypeDef",
+    {
+        "APIVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport/type_defs.pyi` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_importexport.type_defs import ArtifactTypeDef
 
-    data: ArtifactTypeDef = {...}
+    data: ArtifactTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import JobTypeType
@@ -21,29 +21,29 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
-    "CancelJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
-    "GetShippingLabelOutputTypeDef",
     "GetStatusInputRequestTypeDef",
     "JobTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
-    "ListJobsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListJobsInputRequestTypeDef",
     "UpdateJobInputRequestTypeDef",
+    "CancelJobOutputTypeDef",
     "CreateJobOutputTypeDef",
+    "GetShippingLabelOutputTypeDef",
     "GetStatusOutputTypeDef",
     "UpdateJobOutputTypeDef",
     "ListJobsOutputTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
 )
 
 ArtifactTypeDef = TypedDict(
     "ArtifactTypeDef",
     {
         "Description": str,
         "URL": str,
@@ -66,19 +66,22 @@
 )
 
 class CancelJobInputRequestTypeDef(
     _RequiredCancelJobInputRequestTypeDef, _OptionalCancelJobInputRequestTypeDef
 ):
     pass
 
-CancelJobOutputTypeDef = TypedDict(
-    "CancelJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateJobInputRequestTypeDef = TypedDict(
     "_RequiredCreateJobInputRequestTypeDef",
     {
         "JobType": JobTypeType,
@@ -125,23 +128,14 @@
 )
 
 class GetShippingLabelInputRequestTypeDef(
     _RequiredGetShippingLabelInputRequestTypeDef, _OptionalGetShippingLabelInputRequestTypeDef
 ):
     pass
 
-GetShippingLabelOutputTypeDef = TypedDict(
-    "GetShippingLabelOutputTypeDef",
-    {
-        "ShippingLabelURL": str,
-        "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatusInputRequestTypeDef = TypedDict(
     "_RequiredGetStatusInputRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetStatusInputRequestTypeDef = TypedDict(
@@ -164,54 +158,34 @@
         "CreationDate": datetime,
         "IsCanceled": bool,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-ListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "ListJobsInputListJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "APIVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListJobsInputRequestTypeDef = TypedDict(
     "ListJobsInputRequestTypeDef",
     {
         "MaxJobs": int,
         "Marker": str,
         "APIVersion": str,
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
 _RequiredUpdateJobInputRequestTypeDef = TypedDict(
     "_RequiredUpdateJobInputRequestTypeDef",
     {
         "JobId": str,
         "Manifest": str,
         "JobType": JobTypeType,
         "ValidateOnly": bool,
@@ -226,24 +200,41 @@
 )
 
 class UpdateJobInputRequestTypeDef(
     _RequiredUpdateJobInputRequestTypeDef, _OptionalUpdateJobInputRequestTypeDef
 ):
     pass
 
+CancelJobOutputTypeDef = TypedDict(
+    "CancelJobOutputTypeDef",
+    {
+        "Success": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "JobId": str,
         "JobType": JobTypeType,
         "Signature": str,
         "SignatureFileContents": str,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetShippingLabelOutputTypeDef = TypedDict(
+    "GetShippingLabelOutputTypeDef",
+    {
+        "ShippingLabelURL": str,
+        "Warning": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatusOutputTypeDef = TypedDict(
     "GetStatusOutputTypeDef",
     {
         "JobId": str,
@@ -258,29 +249,38 @@
         "LogKey": str,
         "ErrorCount": int,
         "Signature": str,
         "SignatureFileContents": str,
         "CurrentManifest": str,
         "CreationDate": datetime,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobOutputTypeDef = TypedDict(
     "UpdateJobOutputTypeDef",
     {
         "Success": bool,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "IsTruncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "ListJobsInputListJobsPaginateTypeDef",
+    {
+        "APIVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/PKG-INFO` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-importexport
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ImportExport 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ImportExport 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore importexport type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore importexport type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-importexport"></a>
 
 # types-aiobotocore-importexport
 
 [![PyPI - types-aiobotocore-importexport](https://img.shields.io/pypi/v/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-importexport?color=blue)](https://pypistats.org/packages/types-aiobotocore-importexport)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-importexport)](https://pepy.tech/project/types-aiobotocore-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ImportExport 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [types-aiobotocore-importexport docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/).
 
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
@@ -305,44 +304,44 @@
 )
 
 
 def check_value(value: JobTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_importexport.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListJobsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListJobsInputRequestTypeDef,
     UpdateJobInputRequestTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
-def get_structure() -> ArtifactTypeDef:
+def get_value() -> ArtifactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-importexport-2.5.2/types_aiobotocore_importexport.egg-info/SOURCES.txt` & `types-aiobotocore-importexport-2.5.2.post1/types_aiobotocore_importexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*


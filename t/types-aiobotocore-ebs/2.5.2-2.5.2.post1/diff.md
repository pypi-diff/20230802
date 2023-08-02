# Comparing `tmp/types-aiobotocore-ebs-2.5.2.tar.gz` & `tmp/types-aiobotocore-ebs-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ebs-2.5.2.tar", last modified: Sat Jul  8 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-ebs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-ebs-2.5.2.tar` & `types-aiobotocore-ebs-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.154047 types-aiobotocore-ebs-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-07-08 01:43:33.150047 types-aiobotocore-ebs-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:33.154047 types-aiobotocore-ebs-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.142047 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:15.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.150047 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-07-08 01:43:32.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-08 01:43:33.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:32.000000 types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-02 14:36:55.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-02 14:36:56.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-02 14:36:55.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ebs-2.5.2/LICENSE` & `types-aiobotocore-ebs-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2/PKG-INFO` & `types-aiobotocore-ebs-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ebs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ebs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ebs"></a>
 
 # types-aiobotocore-ebs
 
 [![PyPI - types-aiobotocore-ebs](https://img.shields.io/pypi/v/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ebs?color=blue)](https://pypistats.org/packages/types-aiobotocore-ebs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EBS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
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
@@ -281,43 +280,44 @@
 )
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ebs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ebs.type_defs import (
+    BlobTypeDef,
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
-    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockRequestRequestTypeDef,
+    CompleteSnapshotResponseTypeDef,
+    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
+    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
-def get_structure() -> BlockTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ebs-2.5.2/README.md` & `types-aiobotocore-ebs-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ebs"></a>
 
 # types-aiobotocore-ebs
 
 [![PyPI - types-aiobotocore-ebs](https://img.shields.io/pypi/v/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ebs?color=blue)](https://pypistats.org/packages/types-aiobotocore-ebs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EBS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
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
@@ -248,43 +248,44 @@
 )
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ebs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ebs.type_defs import (
+    BlobTypeDef,
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
-    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockRequestRequestTypeDef,
+    CompleteSnapshotResponseTypeDef,
+    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
+    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
-def get_structure() -> BlockTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ebs-2.5.2/setup.py` & `types-aiobotocore-ebs-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ebs",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore ebs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ebs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ebs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/__main__.py` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EBS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.EBS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
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

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/client.py` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
     session = get_session()
     async with session.create_client("ebs") as client:
         client: EBSClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
+    BlobTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotResponseTypeDef,
     TagTypeDef,
@@ -167,15 +167,15 @@
         """
 
     async def put_snapshot_block(
         self,
         *,
         SnapshotId: str,
         BlockIndex: int,
-        BlockData: Union[str, bytes, IO[Any], StreamingBody],
+        BlockData: BlobTypeDef,
         DataLength: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"],
         Progress: int = ...
     ) -> PutSnapshotBlockResponseTypeDef:
         """
         Writes a block of data to a snapshot.
```

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/client.pyi` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
     session = get_session()
     async with session.create_client("ebs") as client:
         client: EBSClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
+    BlobTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotResponseTypeDef,
     TagTypeDef,
@@ -155,15 +155,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#list_snapshot_blocks)
         """
     async def put_snapshot_block(
         self,
         *,
         SnapshotId: str,
         BlockIndex: int,
-        BlockData: Union[str, bytes, IO[Any], StreamingBody],
+        BlockData: BlobTypeDef,
         DataLength: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"],
         Progress: int = ...
     ) -> PutSnapshotBlockResponseTypeDef:
         """
         Writes a block of data to a snapshot.
```

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/literals.py` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/literals.pyi` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/type_defs.py` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ebs service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_ebs.type_defs import BlockTypeDef
+    from types_aiobotocore_ebs.type_defs import BlobTypeDef
 
-    data: BlockTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -26,32 +26,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
-    "CompleteSnapshotResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
-    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
-    "PutSnapshotBlockRequestRequestTypeDef",
-    "PutSnapshotBlockResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "ListSnapshotBlocksResponseTypeDef",
+    "PutSnapshotBlockRequestRequestTypeDef",
+    "CompleteSnapshotResponseTypeDef",
+    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
+    "ListSnapshotBlocksResponseTypeDef",
+    "PutSnapshotBlockResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "BlockIndex": int,
         "BlockToken": str,
     },
     total=False,
@@ -87,42 +89,34 @@
 
 class CompleteSnapshotRequestRequestTypeDef(
     _RequiredCompleteSnapshotRequestRequestTypeDef, _OptionalCompleteSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-CompleteSnapshotResponseTypeDef = TypedDict(
-    "CompleteSnapshotResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetSnapshotBlockRequestRequestTypeDef = TypedDict(
     "GetSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
         "BlockToken": str,
     },
 )
 
-GetSnapshotBlockResponseTypeDef = TypedDict(
-    "GetSnapshotBlockResponseTypeDef",
-    {
-        "DataLength": int,
-        "BlockData": StreamingBody,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChangedBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListChangedBlocksRequestRequestTypeDef",
     {
         "SecondSnapshotId": str,
     },
 )
 _OptionalListChangedBlocksRequestRequestTypeDef = TypedDict(
@@ -163,20 +157,29 @@
 class ListSnapshotBlocksRequestRequestTypeDef(
     _RequiredListSnapshotBlocksRequestRequestTypeDef,
     _OptionalListSnapshotBlocksRequestRequestTypeDef,
 ):
     pass
 
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
-        "BlockData": Union[str, bytes, IO[Any], StreamingBody],
+        "BlockData": BlobTypeDef,
         "DataLength": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 _OptionalPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_OptionalPutSnapshotBlockRequestRequestTypeDef",
@@ -189,64 +192,63 @@
 
 class PutSnapshotBlockRequestRequestTypeDef(
     _RequiredPutSnapshotBlockRequestRequestTypeDef, _OptionalPutSnapshotBlockRequestRequestTypeDef
 ):
     pass
 
 
-PutSnapshotBlockResponseTypeDef = TypedDict(
-    "PutSnapshotBlockResponseTypeDef",
+CompleteSnapshotResponseTypeDef = TypedDict(
+    "CompleteSnapshotResponseTypeDef",
     {
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetSnapshotBlockResponseTypeDef = TypedDict(
+    "GetSnapshotBlockResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DataLength": int,
+        "BlockData": StreamingBody,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ListChangedBlocksResponseTypeDef = TypedDict(
+    "ListChangedBlocksResponseTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "ChangedBlocks": List[ChangedBlockTypeDef],
+        "ExpiryTime": datetime,
+        "VolumeSize": int,
+        "BlockSize": int,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListSnapshotBlocksResponseTypeDef = TypedDict(
     "ListSnapshotBlocksResponseTypeDef",
     {
         "Blocks": List[BlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListChangedBlocksResponseTypeDef = TypedDict(
-    "ListChangedBlocksResponseTypeDef",
+PutSnapshotBlockResponseTypeDef = TypedDict(
+    "PutSnapshotBlockResponseTypeDef",
     {
-        "ChangedBlocks": List[ChangedBlockTypeDef],
-        "ExpiryTime": datetime,
-        "VolumeSize": int,
-        "BlockSize": int,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredStartSnapshotRequestRequestTypeDef",
     {
         "VolumeSize": int,
@@ -282,10 +284,10 @@
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "Tags": List[TagTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs/type_defs.pyi` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ebs service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_ebs.type_defs import BlockTypeDef
+    from types_aiobotocore_ebs.type_defs import BlobTypeDef
 
-    data: BlockTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -25,32 +25,34 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
-    "CompleteSnapshotResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
-    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
-    "PutSnapshotBlockRequestRequestTypeDef",
-    "PutSnapshotBlockResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "ListSnapshotBlocksResponseTypeDef",
+    "PutSnapshotBlockRequestRequestTypeDef",
+    "CompleteSnapshotResponseTypeDef",
+    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
+    "ListSnapshotBlocksResponseTypeDef",
+    "PutSnapshotBlockResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "BlockIndex": int,
         "BlockToken": str,
     },
     total=False,
@@ -84,42 +86,34 @@
 )
 
 class CompleteSnapshotRequestRequestTypeDef(
     _RequiredCompleteSnapshotRequestRequestTypeDef, _OptionalCompleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-CompleteSnapshotResponseTypeDef = TypedDict(
-    "CompleteSnapshotResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetSnapshotBlockRequestRequestTypeDef = TypedDict(
     "GetSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
         "BlockToken": str,
     },
 )
 
-GetSnapshotBlockResponseTypeDef = TypedDict(
-    "GetSnapshotBlockResponseTypeDef",
-    {
-        "DataLength": int,
-        "BlockData": StreamingBody,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChangedBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListChangedBlocksRequestRequestTypeDef",
     {
         "SecondSnapshotId": str,
     },
 )
 _OptionalListChangedBlocksRequestRequestTypeDef = TypedDict(
@@ -156,20 +150,29 @@
 
 class ListSnapshotBlocksRequestRequestTypeDef(
     _RequiredListSnapshotBlocksRequestRequestTypeDef,
     _OptionalListSnapshotBlocksRequestRequestTypeDef,
 ):
     pass
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
-        "BlockData": Union[str, bytes, IO[Any], StreamingBody],
+        "BlockData": BlobTypeDef,
         "DataLength": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 _OptionalPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_OptionalPutSnapshotBlockRequestRequestTypeDef",
@@ -180,64 +183,63 @@
 )
 
 class PutSnapshotBlockRequestRequestTypeDef(
     _RequiredPutSnapshotBlockRequestRequestTypeDef, _OptionalPutSnapshotBlockRequestRequestTypeDef
 ):
     pass
 
-PutSnapshotBlockResponseTypeDef = TypedDict(
-    "PutSnapshotBlockResponseTypeDef",
+CompleteSnapshotResponseTypeDef = TypedDict(
+    "CompleteSnapshotResponseTypeDef",
     {
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetSnapshotBlockResponseTypeDef = TypedDict(
+    "GetSnapshotBlockResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DataLength": int,
+        "BlockData": StreamingBody,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ListChangedBlocksResponseTypeDef = TypedDict(
+    "ListChangedBlocksResponseTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "ChangedBlocks": List[ChangedBlockTypeDef],
+        "ExpiryTime": datetime,
+        "VolumeSize": int,
+        "BlockSize": int,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListSnapshotBlocksResponseTypeDef = TypedDict(
     "ListSnapshotBlocksResponseTypeDef",
     {
         "Blocks": List[BlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListChangedBlocksResponseTypeDef = TypedDict(
-    "ListChangedBlocksResponseTypeDef",
+PutSnapshotBlockResponseTypeDef = TypedDict(
+    "PutSnapshotBlockResponseTypeDef",
     {
-        "ChangedBlocks": List[ChangedBlockTypeDef],
-        "ExpiryTime": datetime,
-        "VolumeSize": int,
-        "BlockSize": int,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredStartSnapshotRequestRequestTypeDef",
     {
         "VolumeSize": int,
@@ -271,10 +273,10 @@
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "Tags": List[TagTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/PKG-INFO` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ebs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ebs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ebs"></a>
 
 # types-aiobotocore-ebs
 
 [![PyPI - types-aiobotocore-ebs](https://img.shields.io/pypi/v/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ebs?color=blue)](https://pypistats.org/packages/types-aiobotocore-ebs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EBS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
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
@@ -281,43 +280,44 @@
 )
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ebs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ebs.type_defs import (
+    BlobTypeDef,
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
-    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockRequestRequestTypeDef,
+    CompleteSnapshotResponseTypeDef,
+    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
+    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
-def get_structure() -> BlockTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ebs-2.5.2/types_aiobotocore_ebs.egg-info/SOURCES.txt` & `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


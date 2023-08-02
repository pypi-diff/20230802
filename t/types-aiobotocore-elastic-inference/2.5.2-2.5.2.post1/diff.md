# Comparing `tmp/types-aiobotocore-elastic-inference-2.5.2.tar.gz` & `tmp/types-aiobotocore-elastic-inference-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastic-inference-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastic-inference-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-elastic-inference-2.5.2.tar` & `types-aiobotocore-elastic-inference-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.246086 types-aiobotocore-elastic-inference-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-08 01:43:35.238086 types-aiobotocore-elastic-inference-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.246086 types-aiobotocore-elastic-inference-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.238086 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:18.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.238086 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-08 01:43:35.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:35.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:35.000000 types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.605594 types-aiobotocore-elastic-inference-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-08-02 14:52:14.601594 types-aiobotocore-elastic-inference-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.605594 types-aiobotocore-elastic-inference-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.601594 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-02 14:38:07.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.601594 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/LICENSE` & `types-aiobotocore-elastic-inference-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/PKG-INFO` & `types-aiobotocore-elastic-inference-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elastic-inference type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elastic-inference type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elastic-inference"></a>
 
 # types-aiobotocore-elastic-inference
 
 [![PyPI - types-aiobotocore-elastic-inference](https://img.shields.io/pypi/v/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastic-inference?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastic-inference)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticInference 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
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
@@ -308,46 +307,46 @@
 )
 
 
 def check_value(value: DescribeAcceleratorsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elastic_inference.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elastic_inference.type_defs import (
     AcceleratorTypeOfferingTypeDef,
     KeyValuePairTypeDef,
     MemoryInfoTypeDef,
     DescribeAcceleratorOfferingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     ElasticInferenceAcceleratorHealthTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
     AcceleratorTypeTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
+    DescribeAcceleratorOfferingsResponseTypeDef,
+    ListTagsForResourceResultTypeDef,
     DescribeAcceleratorsRequestRequestTypeDef,
+    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
     ElasticInferenceAcceleratorTypeDef,
     DescribeAcceleratorTypesResponseTypeDef,
     DescribeAcceleratorsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceleratorTypeOfferingTypeDef:
+def get_value() -> AcceleratorTypeOfferingTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/README.md` & `types-aiobotocore-elastic-inference-2.5.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-elastic-inference"></a>
 
 # types-aiobotocore-elastic-inference
 
 [![PyPI - types-aiobotocore-elastic-inference](https://img.shields.io/pypi/v/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastic-inference?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastic-inference)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticInference 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
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
@@ -275,46 +275,46 @@
 )
 
 
 def check_value(value: DescribeAcceleratorsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elastic_inference.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elastic_inference.type_defs import (
     AcceleratorTypeOfferingTypeDef,
     KeyValuePairTypeDef,
     MemoryInfoTypeDef,
     DescribeAcceleratorOfferingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     ElasticInferenceAcceleratorHealthTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
     AcceleratorTypeTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
+    DescribeAcceleratorOfferingsResponseTypeDef,
+    ListTagsForResourceResultTypeDef,
     DescribeAcceleratorsRequestRequestTypeDef,
+    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
     ElasticInferenceAcceleratorTypeDef,
     DescribeAcceleratorTypesResponseTypeDef,
     DescribeAcceleratorsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceleratorTypeOfferingTypeDef:
+def get_value() -> AcceleratorTypeOfferingTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/setup.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastic-inference",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with"
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
-        "aiobotocore elastic-inference type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore elastic-inference type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elastic_inference": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/"
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/__init__.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/__init__.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/__main__.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticInference 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ElasticInference 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/client.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/client.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/literals.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/literals.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/paginator.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,13 +47,13 @@
     """
 
     def paginate(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/paginators/#describeacceleratorspaginator)
         """
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/paginator.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     """
 
     def paginate(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/paginators/#describeacceleratorspaginator)
         """
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/type_defs.py` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeOfferingTypeDef
 
-    data: AcceleratorTypeOfferingTypeDef = {...}
+    data: AcceleratorTypeOfferingTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import LocationTypeType
 
@@ -23,26 +23,26 @@
 
 
 __all__ = (
     "AcceleratorTypeOfferingTypeDef",
     "KeyValuePairTypeDef",
     "MemoryInfoTypeDef",
     "DescribeAcceleratorOfferingsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ElasticInferenceAcceleratorHealthTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "DescribeAcceleratorOfferingsResponseTypeDef",
     "AcceleratorTypeTypeDef",
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    "DescribeAcceleratorOfferingsResponseTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "DescribeAcceleratorsRequestRequestTypeDef",
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
     "ElasticInferenceAcceleratorTypeDef",
     "DescribeAcceleratorTypesResponseTypeDef",
     "DescribeAcceleratorsResponseTypeDef",
 )
 
 AcceleratorTypeOfferingTypeDef = TypedDict(
     "AcceleratorTypeOfferingTypeDef",
@@ -89,23 +89,44 @@
 class DescribeAcceleratorOfferingsRequestRequestTypeDef(
     _RequiredDescribeAcceleratorOfferingsRequestRequestTypeDef,
     _OptionalDescribeAcceleratorOfferingsRequestRequestTypeDef,
 ):
     pass
 
 
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorHealthTypeDef = TypedDict(
     "ElasticInferenceAcceleratorHealthTypeDef",
     {
         "status": str,
     },
     total=False,
 )
@@ -113,43 +134,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -158,53 +150,61 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
-    "DescribeAcceleratorOfferingsResponseTypeDef",
-    {
-        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AcceleratorTypeTypeDef = TypedDict(
     "AcceleratorTypeTypeDef",
     {
         "acceleratorTypeName": str,
         "memoryInfo": MemoryInfoTypeDef,
         "throughputInfo": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
+    "DescribeAcceleratorOfferingsResponseTypeDef",
     {
-        "acceleratorIds": Sequence[str],
-        "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeAcceleratorsRequestRequestTypeDef = TypedDict(
     "DescribeAcceleratorsRequestRequestTypeDef",
     {
         "acceleratorIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    {
+        "acceleratorIds": Sequence[str],
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorTypeDef = TypedDict(
     "ElasticInferenceAcceleratorTypeDef",
     {
         "acceleratorHealth": ElasticInferenceAcceleratorHealthTypeDef,
         "acceleratorType": str,
         "acceleratorId": str,
         "availabilityZone": str,
@@ -213,19 +213,19 @@
     total=False,
 )
 
 DescribeAcceleratorTypesResponseTypeDef = TypedDict(
     "DescribeAcceleratorTypesResponseTypeDef",
     {
         "acceleratorTypes": List[AcceleratorTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAcceleratorsResponseTypeDef = TypedDict(
     "DescribeAcceleratorsResponseTypeDef",
     {
         "acceleratorSet": List[ElasticInferenceAcceleratorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference/type_defs.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeOfferingTypeDef
 
-    data: AcceleratorTypeOfferingTypeDef = {...}
+    data: AcceleratorTypeOfferingTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import LocationTypeType
 
@@ -22,26 +22,26 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceleratorTypeOfferingTypeDef",
     "KeyValuePairTypeDef",
     "MemoryInfoTypeDef",
     "DescribeAcceleratorOfferingsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ElasticInferenceAcceleratorHealthTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "DescribeAcceleratorOfferingsResponseTypeDef",
     "AcceleratorTypeTypeDef",
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    "DescribeAcceleratorOfferingsResponseTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "DescribeAcceleratorsRequestRequestTypeDef",
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
     "ElasticInferenceAcceleratorTypeDef",
     "DescribeAcceleratorTypesResponseTypeDef",
     "DescribeAcceleratorsResponseTypeDef",
 )
 
 AcceleratorTypeOfferingTypeDef = TypedDict(
     "AcceleratorTypeOfferingTypeDef",
@@ -86,23 +86,44 @@
 
 class DescribeAcceleratorOfferingsRequestRequestTypeDef(
     _RequiredDescribeAcceleratorOfferingsRequestRequestTypeDef,
     _OptionalDescribeAcceleratorOfferingsRequestRequestTypeDef,
 ):
     pass
 
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorHealthTypeDef = TypedDict(
     "ElasticInferenceAcceleratorHealthTypeDef",
     {
         "status": str,
     },
     total=False,
 )
@@ -110,43 +131,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -155,53 +147,61 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
-    "DescribeAcceleratorOfferingsResponseTypeDef",
-    {
-        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AcceleratorTypeTypeDef = TypedDict(
     "AcceleratorTypeTypeDef",
     {
         "acceleratorTypeName": str,
         "memoryInfo": MemoryInfoTypeDef,
         "throughputInfo": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
+    "DescribeAcceleratorOfferingsResponseTypeDef",
     {
-        "acceleratorIds": Sequence[str],
-        "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeAcceleratorsRequestRequestTypeDef = TypedDict(
     "DescribeAcceleratorsRequestRequestTypeDef",
     {
         "acceleratorIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    {
+        "acceleratorIds": Sequence[str],
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorTypeDef = TypedDict(
     "ElasticInferenceAcceleratorTypeDef",
     {
         "acceleratorHealth": ElasticInferenceAcceleratorHealthTypeDef,
         "acceleratorType": str,
         "acceleratorId": str,
         "availabilityZone": str,
@@ -210,19 +210,19 @@
     total=False,
 )
 
 DescribeAcceleratorTypesResponseTypeDef = TypedDict(
     "DescribeAcceleratorTypesResponseTypeDef",
     {
         "acceleratorTypes": List[AcceleratorTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAcceleratorsResponseTypeDef = TypedDict(
     "DescribeAcceleratorsResponseTypeDef",
     {
         "acceleratorSet": List[ElasticInferenceAcceleratorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/PKG-INFO` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elastic-inference type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elastic-inference type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elastic-inference"></a>
 
 # types-aiobotocore-elastic-inference
 
 [![PyPI - types-aiobotocore-elastic-inference](https://img.shields.io/pypi/v/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastic-inference?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastic-inference)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticInference 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
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
@@ -308,46 +307,46 @@
 )
 
 
 def check_value(value: DescribeAcceleratorsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elastic_inference.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elastic_inference.type_defs import (
     AcceleratorTypeOfferingTypeDef,
     KeyValuePairTypeDef,
     MemoryInfoTypeDef,
     DescribeAcceleratorOfferingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     ElasticInferenceAcceleratorHealthTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
     AcceleratorTypeTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
+    DescribeAcceleratorOfferingsResponseTypeDef,
+    ListTagsForResourceResultTypeDef,
     DescribeAcceleratorsRequestRequestTypeDef,
+    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
     ElasticInferenceAcceleratorTypeDef,
     DescribeAcceleratorTypesResponseTypeDef,
     DescribeAcceleratorsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceleratorTypeOfferingTypeDef:
+def get_value() -> AcceleratorTypeOfferingTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt` & `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*


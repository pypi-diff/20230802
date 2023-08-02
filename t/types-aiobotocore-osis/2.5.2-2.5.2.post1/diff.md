# Comparing `tmp/types-aiobotocore-osis-2.5.2.tar.gz` & `tmp/types-aiobotocore-osis-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-osis-2.5.2.tar", last modified: Sat Jul  8 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-osis-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
```

## Comparing `types-aiobotocore-osis-2.5.2.tar` & `types-aiobotocore-osis-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.018645 types-aiobotocore-osis-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-08 01:44:05.014645 types-aiobotocore-osis-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:05.018645 types-aiobotocore-osis-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.010645 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:13.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.014645 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-08 01:44:04.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-08 01:44:04.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:04.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:44:04.000000 types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.661504 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-osis-2.5.2/LICENSE` & `types-aiobotocore-osis-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-osis-2.5.2/PKG-INFO` & `types-aiobotocore-osis-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-osis
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore osis type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore osis type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-osis"></a>
 
 # types-aiobotocore-osis
 
 [![PyPI - types-aiobotocore-osis](https://img.shields.io/pypi/v/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-osis?color=blue)](https://pypistats.org/packages/types-aiobotocore-osis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-osis)](https://pepy.tech/project/types-aiobotocore-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpenSearchIngestion 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
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
@@ -282,65 +281,67 @@
 )
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_osis.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
+    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PipelineStatusReasonTypeDef,
-    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
+    VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
     LogPublishingOptionsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    VpcEndpointTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcEndpointTypeDef,
+    VpcOptionsUnionTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    PipelineTypeDef,
     ListPipelinesResponseTypeDef,
+    PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ChangeProgressStageTypeDef:
+def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-osis-2.5.2/README.md` & `types-aiobotocore-osis-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-osis"></a>
 
 # types-aiobotocore-osis
 
 [![PyPI - types-aiobotocore-osis](https://img.shields.io/pypi/v/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-osis?color=blue)](https://pypistats.org/packages/types-aiobotocore-osis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-osis)](https://pepy.tech/project/types-aiobotocore-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpenSearchIngestion 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
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
@@ -249,65 +249,67 @@
 )
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_osis.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
+    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PipelineStatusReasonTypeDef,
-    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
+    VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
     LogPublishingOptionsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    VpcEndpointTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcEndpointTypeDef,
+    VpcOptionsUnionTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    PipelineTypeDef,
     ListPipelinesResponseTypeDef,
+    PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ChangeProgressStageTypeDef:
+def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-osis-2.5.2/setup.py` & `types-aiobotocore-osis-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-osis",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with"
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
-    keywords="aiobotocore osis type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore osis type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_osis": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/__main__.py` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.OpenSearchIngestion 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
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

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/client.py` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
-    VpcOptionsTypeDef,
+    VpcOptionsUnionTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -96,15 +96,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: VpcOptionsTypeDef = ...,
+        VpcOptions: VpcOptionsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#create_pipeline)
```

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/client.pyi` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
-    VpcOptionsTypeDef,
+    VpcOptionsUnionTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -90,15 +90,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: VpcOptionsTypeDef = ...,
+        VpcOptions: VpcOptionsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#create_pipeline)
```

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/literals.py` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/literals.pyi` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/type_defs.py` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
-    data: ChangeProgressStageTypeDef = {...}
+    data: ChangeProgressStageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ChangeProgressStageStatusesType,
     ChangeProgressStatusesType,
     PipelineStatusType,
 )
 
@@ -28,43 +28,45 @@
 
 
 __all__ = (
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
+    "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PipelineStatusReasonTypeDef",
-    "ResponseMetadataTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
+    "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
     "LogPublishingOptionsTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "VpcEndpointTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
+    "VpcEndpointTypeDef",
+    "VpcOptionsUnionTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "PipelineTypeDef",
     "ListPipelinesResponseTypeDef",
+    "PipelineTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
     "StartPipelineResponseTypeDef",
     "StopPipelineResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
 )
 
@@ -109,14 +111,25 @@
 )
 
 
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
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
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -178,25 +191,14 @@
     "PipelineStatusReasonTypeDef",
     {
         "Description": str,
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
 StartPipelineRequestRequestTypeDef = TypedDict(
     "StartPipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -226,14 +228,33 @@
     "ValidationMessageTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+_RequiredVpcOptionsOutputTypeDef = TypedDict(
+    "_RequiredVpcOptionsOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+    },
+)
+_OptionalVpcOptionsOutputTypeDef = TypedDict(
+    "_OptionalVpcOptionsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+
+class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
+    pass
+
+
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
@@ -246,53 +267,43 @@
     {
         "IsLoggingEnabled": bool,
         "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
     total=False,
 )
 
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
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-VpcEndpointTypeDef = TypedDict(
-    "VpcEndpointTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "VpcOptions": VpcOptionsTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelineBlueprintsResponseTypeDef = TypedDict(
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
@@ -308,23 +319,34 @@
 )
 
 ValidatePipelineResponseTypeDef = TypedDict(
     "ValidatePipelineResponseTypeDef",
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VpcEndpointTypeDef = TypedDict(
+    "VpcEndpointTypeDef",
+    {
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "VpcOptions": VpcOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+VpcOptionsUnionTypeDef = Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef]
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
@@ -370,14 +392,23 @@
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
 
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Pipelines": List[PipelineSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
@@ -389,55 +420,46 @@
         "IngestEndpointUrls": List[str],
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPipelineResponseTypeDef = TypedDict(
     "GetPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartPipelineResponseTypeDef = TypedDict(
     "StartPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopPipelineResponseTypeDef = TypedDict(
     "StopPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis/type_defs.pyi` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
-    data: ChangeProgressStageTypeDef = {...}
+    data: ChangeProgressStageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ChangeProgressStageStatusesType,
     ChangeProgressStatusesType,
     PipelineStatusType,
 )
 
@@ -27,43 +27,45 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
+    "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PipelineStatusReasonTypeDef",
-    "ResponseMetadataTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
+    "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
     "LogPublishingOptionsTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "VpcEndpointTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
+    "VpcEndpointTypeDef",
+    "VpcOptionsUnionTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "PipelineTypeDef",
     "ListPipelinesResponseTypeDef",
+    "PipelineTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
     "StartPipelineResponseTypeDef",
     "StopPipelineResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
 )
 
@@ -106,14 +108,25 @@
     },
     total=False,
 )
 
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
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
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -175,25 +188,14 @@
     "PipelineStatusReasonTypeDef",
     {
         "Description": str,
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
 StartPipelineRequestRequestTypeDef = TypedDict(
     "StartPipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -223,14 +225,31 @@
     "ValidationMessageTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+_RequiredVpcOptionsOutputTypeDef = TypedDict(
+    "_RequiredVpcOptionsOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+    },
+)
+_OptionalVpcOptionsOutputTypeDef = TypedDict(
+    "_OptionalVpcOptionsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
+    pass
+
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
@@ -243,53 +262,43 @@
     {
         "IsLoggingEnabled": bool,
         "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
     total=False,
 )
 
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
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-VpcEndpointTypeDef = TypedDict(
-    "VpcEndpointTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "VpcOptions": VpcOptionsTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelineBlueprintsResponseTypeDef = TypedDict(
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
@@ -305,23 +314,34 @@
 )
 
 ValidatePipelineResponseTypeDef = TypedDict(
     "ValidatePipelineResponseTypeDef",
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VpcEndpointTypeDef = TypedDict(
+    "VpcEndpointTypeDef",
+    {
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "VpcOptions": VpcOptionsOutputTypeDef,
     },
+    total=False,
 )
 
+VpcOptionsUnionTypeDef = Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef]
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
@@ -363,14 +383,23 @@
 )
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Pipelines": List[PipelineSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
@@ -382,55 +411,46 @@
         "IngestEndpointUrls": List[str],
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPipelineResponseTypeDef = TypedDict(
     "GetPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartPipelineResponseTypeDef = TypedDict(
     "StartPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopPipelineResponseTypeDef = TypedDict(
     "StopPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/PKG-INFO` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-osis
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore osis type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore osis type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-osis"></a>
 
 # types-aiobotocore-osis
 
 [![PyPI - types-aiobotocore-osis](https://img.shields.io/pypi/v/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-osis?color=blue)](https://pypistats.org/packages/types-aiobotocore-osis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-osis)](https://pepy.tech/project/types-aiobotocore-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpenSearchIngestion 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
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
@@ -282,65 +281,67 @@
 )
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_osis.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
+    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PipelineStatusReasonTypeDef,
-    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
+    VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
     LogPublishingOptionsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    VpcEndpointTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcEndpointTypeDef,
+    VpcOptionsUnionTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    PipelineTypeDef,
     ListPipelinesResponseTypeDef,
+    PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ChangeProgressStageTypeDef:
+def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-osis-2.5.2/types_aiobotocore_osis.egg-info/SOURCES.txt` & `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-synthetics-2.5.2.tar.gz` & `tmp/types-aiobotocore-synthetics-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-synthetics-2.5.2.tar", last modified: Sat Jul  8 01:44:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-synthetics-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
```

## Comparing `types-aiobotocore-synthetics-2.5.2.tar` & `types-aiobotocore-synthetics-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.118991 types-aiobotocore-synthetics-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-08 01:44:25.118991 types-aiobotocore-synthetics-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:25.118991 types-aiobotocore-synthetics-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.114991 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18358 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:54.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.118991 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-08 01:44:24.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-08 01:44:24.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:24.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:44:24.000000 types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18881 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-synthetics-2.5.2/LICENSE` & `types-aiobotocore-synthetics-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2/PKG-INFO` & `types-aiobotocore-synthetics-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-synthetics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore synthetics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore synthetics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-synthetics"></a>
 
 # types-aiobotocore-synthetics
 
 [![PyPI - types-aiobotocore-synthetics](https://img.shields.io/pypi/v/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-synthetics?color=blue)](https://pypistats.org/packages/types-aiobotocore-synthetics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-synthetics)](https://pepy.tech/project/types-aiobotocore-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Synthetics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
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
@@ -285,38 +284,40 @@
 )
 
 
 def check_value(value: CanaryRunStateReasonCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_synthetics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
-    CanaryCodeInputTypeDef,
+    BlobTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
     CanaryRunStatusTypeDef,
     CanaryRunTimelineTypeDef,
     CanaryScheduleInputTypeDef,
     CanaryScheduleOutputTypeDef,
     CanaryStatusTypeDef,
     CanaryTimelineTypeDef,
     VpcConfigOutputTypeDef,
     VpcConfigInputTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     DeleteCanaryRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DescribeCanariesLastRunRequestRequestTypeDef,
     DescribeCanariesRequestRequestTypeDef,
     DescribeRuntimeVersionsRequestRequestTypeDef,
@@ -324,46 +325,46 @@
     DisassociateResourceRequestRequestTypeDef,
     GetCanaryRequestRequestTypeDef,
     GetCanaryRunsRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GroupSummaryTypeDef,
     ListAssociatedGroupsRequestRequestTypeDef,
     ListGroupResourcesRequestRequestTypeDef,
-    ListGroupResourcesResponseTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartCanaryRequestRequestTypeDef,
     StopCanaryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArtifactConfigInputTypeDef,
     ArtifactConfigOutputTypeDef,
-    VisualReferenceInputTypeDef,
     VisualReferenceOutputTypeDef,
+    VisualReferenceInputTypeDef,
+    CanaryCodeInputTypeDef,
     CanaryRunTypeDef,
+    ListGroupResourcesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     DescribeRuntimeVersionsResponseTypeDef,
     ListAssociatedGroupsResponseTypeDef,
     ListGroupsResponseTypeDef,
+    CanaryTypeDef,
     CreateCanaryRequestRequestTypeDef,
     UpdateCanaryRequestRequestTypeDef,
-    CanaryTypeDef,
     CanaryLastRunTypeDef,
     GetCanaryRunsResponseTypeDef,
     CreateCanaryResponseTypeDef,
     DescribeCanariesResponseTypeDef,
     GetCanaryResponseTypeDef,
     DescribeCanariesLastRunResponseTypeDef,
 )
 
 
-def get_structure() -> S3EncryptionConfigTypeDef:
+def get_value() -> S3EncryptionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-synthetics-2.5.2/README.md` & `types-aiobotocore-synthetics-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-synthetics"></a>
 
 # types-aiobotocore-synthetics
 
 [![PyPI - types-aiobotocore-synthetics](https://img.shields.io/pypi/v/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-synthetics?color=blue)](https://pypistats.org/packages/types-aiobotocore-synthetics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-synthetics)](https://pepy.tech/project/types-aiobotocore-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Synthetics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
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
@@ -252,38 +252,40 @@
 )
 
 
 def check_value(value: CanaryRunStateReasonCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_synthetics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
-    CanaryCodeInputTypeDef,
+    BlobTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
     CanaryRunStatusTypeDef,
     CanaryRunTimelineTypeDef,
     CanaryScheduleInputTypeDef,
     CanaryScheduleOutputTypeDef,
     CanaryStatusTypeDef,
     CanaryTimelineTypeDef,
     VpcConfigOutputTypeDef,
     VpcConfigInputTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     DeleteCanaryRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DescribeCanariesLastRunRequestRequestTypeDef,
     DescribeCanariesRequestRequestTypeDef,
     DescribeRuntimeVersionsRequestRequestTypeDef,
@@ -291,46 +293,46 @@
     DisassociateResourceRequestRequestTypeDef,
     GetCanaryRequestRequestTypeDef,
     GetCanaryRunsRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GroupSummaryTypeDef,
     ListAssociatedGroupsRequestRequestTypeDef,
     ListGroupResourcesRequestRequestTypeDef,
-    ListGroupResourcesResponseTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartCanaryRequestRequestTypeDef,
     StopCanaryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArtifactConfigInputTypeDef,
     ArtifactConfigOutputTypeDef,
-    VisualReferenceInputTypeDef,
     VisualReferenceOutputTypeDef,
+    VisualReferenceInputTypeDef,
+    CanaryCodeInputTypeDef,
     CanaryRunTypeDef,
+    ListGroupResourcesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     DescribeRuntimeVersionsResponseTypeDef,
     ListAssociatedGroupsResponseTypeDef,
     ListGroupsResponseTypeDef,
+    CanaryTypeDef,
     CreateCanaryRequestRequestTypeDef,
     UpdateCanaryRequestRequestTypeDef,
-    CanaryTypeDef,
     CanaryLastRunTypeDef,
     GetCanaryRunsResponseTypeDef,
     CreateCanaryResponseTypeDef,
     DescribeCanariesResponseTypeDef,
     GetCanaryResponseTypeDef,
     DescribeCanariesLastRunResponseTypeDef,
 )
 
 
-def get_structure() -> S3EncryptionConfigTypeDef:
+def get_value() -> S3EncryptionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-synthetics-2.5.2/setup.py` & `types-aiobotocore-synthetics-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-synthetics",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_synthetics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Synthetics 2.5.2 service generated with"
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
-    keywords="aiobotocore synthetics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore synthetics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_synthetics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/"
```

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/__main__.py` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Synthetics 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Synthetics 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics\nOther"
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

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/client.py` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/client.pyi` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/literals.py` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/literals.pyi` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/type_defs.py` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_synthetics.type_defs import S3EncryptionConfigTypeDef
 
-    data: S3EncryptionConfigTypeDef = {...}
+    data: S3EncryptionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -30,27 +30,29 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
     "AssociateResourceRequestRequestTypeDef",
+    "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
-    "CanaryCodeInputTypeDef",
+    "BlobTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
     "CanaryRunStatusTypeDef",
     "CanaryRunTimelineTypeDef",
     "CanaryScheduleInputTypeDef",
     "CanaryScheduleOutputTypeDef",
     "CanaryStatusTypeDef",
     "CanaryTimelineTypeDef",
     "VpcConfigOutputTypeDef",
     "VpcConfigInputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
     "DeleteCanaryRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DescribeCanariesLastRunRequestRequestTypeDef",
     "DescribeCanariesRequestRequestTypeDef",
     "DescribeRuntimeVersionsRequestRequestTypeDef",
@@ -58,36 +60,36 @@
     "DisassociateResourceRequestRequestTypeDef",
     "GetCanaryRequestRequestTypeDef",
     "GetCanaryRunsRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GroupSummaryTypeDef",
     "ListAssociatedGroupsRequestRequestTypeDef",
     "ListGroupResourcesRequestRequestTypeDef",
-    "ListGroupResourcesResponseTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartCanaryRequestRequestTypeDef",
     "StopCanaryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArtifactConfigInputTypeDef",
     "ArtifactConfigOutputTypeDef",
-    "VisualReferenceInputTypeDef",
     "VisualReferenceOutputTypeDef",
+    "VisualReferenceInputTypeDef",
+    "CanaryCodeInputTypeDef",
     "CanaryRunTypeDef",
+    "ListGroupResourcesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "DescribeRuntimeVersionsResponseTypeDef",
     "ListAssociatedGroupsResponseTypeDef",
     "ListGroupsResponseTypeDef",
+    "CanaryTypeDef",
     "CreateCanaryRequestRequestTypeDef",
     "UpdateCanaryRequestRequestTypeDef",
-    "CanaryTypeDef",
     "CanaryLastRunTypeDef",
     "GetCanaryRunsResponseTypeDef",
     "CreateCanaryResponseTypeDef",
     "DescribeCanariesResponseTypeDef",
     "GetCanaryResponseTypeDef",
     "DescribeCanariesLastRunResponseTypeDef",
 )
@@ -105,55 +107,55 @@
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
 
-_RequiredBaseScreenshotTypeDef = TypedDict(
-    "_RequiredBaseScreenshotTypeDef",
+_RequiredBaseScreenshotOutputTypeDef = TypedDict(
+    "_RequiredBaseScreenshotOutputTypeDef",
     {
         "ScreenshotName": str,
     },
 )
-_OptionalBaseScreenshotTypeDef = TypedDict(
-    "_OptionalBaseScreenshotTypeDef",
+_OptionalBaseScreenshotOutputTypeDef = TypedDict(
+    "_OptionalBaseScreenshotOutputTypeDef",
     {
         "IgnoreCoordinates": List[str],
     },
     total=False,
 )
 
 
-class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
+class BaseScreenshotOutputTypeDef(
+    _RequiredBaseScreenshotOutputTypeDef, _OptionalBaseScreenshotOutputTypeDef
+):
     pass
 
 
-_RequiredCanaryCodeInputTypeDef = TypedDict(
-    "_RequiredCanaryCodeInputTypeDef",
+_RequiredBaseScreenshotTypeDef = TypedDict(
+    "_RequiredBaseScreenshotTypeDef",
     {
-        "Handler": str,
+        "ScreenshotName": str,
     },
 )
-_OptionalCanaryCodeInputTypeDef = TypedDict(
-    "_OptionalCanaryCodeInputTypeDef",
+_OptionalBaseScreenshotTypeDef = TypedDict(
+    "_OptionalBaseScreenshotTypeDef",
     {
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3Version": str,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
+        "IgnoreCoordinates": Sequence[str],
     },
     total=False,
 )
 
 
-class CanaryCodeInputTypeDef(_RequiredCanaryCodeInputTypeDef, _OptionalCanaryCodeInputTypeDef):
+class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CanaryCodeOutputTypeDef = TypedDict(
     "CanaryCodeOutputTypeDef",
     {
         "SourceLocationArn": str,
         "Handler": str,
     },
     total=False,
@@ -265,14 +267,25 @@
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
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
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateGroupRequestRequestTypeDef = TypedDict(
@@ -467,23 +480,14 @@
 class ListGroupResourcesRequestRequestTypeDef(
     _RequiredListGroupResourcesRequestRequestTypeDef,
     _OptionalListGroupResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-ListGroupResourcesResponseTypeDef = TypedDict(
-    "ListGroupResourcesResponseTypeDef",
-    {
-        "Resources": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -492,33 +496,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
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
 StartCanaryRequestRequestTypeDef = TypedDict(
     "StartCanaryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -557,14 +542,23 @@
     "ArtifactConfigOutputTypeDef",
     {
         "S3Encryption": S3EncryptionConfigTypeDef,
     },
     total=False,
 )
 
+VisualReferenceOutputTypeDef = TypedDict(
+    "VisualReferenceOutputTypeDef",
+    {
+        "BaseScreenshots": List[BaseScreenshotOutputTypeDef],
+        "BaseCanaryRunId": str,
+    },
+    total=False,
+)
+
 _RequiredVisualReferenceInputTypeDef = TypedDict(
     "_RequiredVisualReferenceInputTypeDef",
     {
         "BaseCanaryRunId": str,
     },
 )
 _OptionalVisualReferenceInputTypeDef = TypedDict(
@@ -578,76 +572,130 @@
 
 class VisualReferenceInputTypeDef(
     _RequiredVisualReferenceInputTypeDef, _OptionalVisualReferenceInputTypeDef
 ):
     pass
 
 
-VisualReferenceOutputTypeDef = TypedDict(
-    "VisualReferenceOutputTypeDef",
+_RequiredCanaryCodeInputTypeDef = TypedDict(
+    "_RequiredCanaryCodeInputTypeDef",
     {
-        "BaseScreenshots": List[BaseScreenshotTypeDef],
-        "BaseCanaryRunId": str,
+        "Handler": str,
+    },
+)
+_OptionalCanaryCodeInputTypeDef = TypedDict(
+    "_OptionalCanaryCodeInputTypeDef",
+    {
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3Version": str,
+        "ZipFile": BlobTypeDef,
     },
     total=False,
 )
 
+
+class CanaryCodeInputTypeDef(_RequiredCanaryCodeInputTypeDef, _OptionalCanaryCodeInputTypeDef):
+    pass
+
+
 CanaryRunTypeDef = TypedDict(
     "CanaryRunTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": CanaryRunStatusTypeDef,
         "Timeline": CanaryRunTimelineTypeDef,
         "ArtifactS3Location": str,
     },
     total=False,
 )
 
+ListGroupResourcesResponseTypeDef = TypedDict(
+    "ListGroupResourcesResponseTypeDef",
+    {
+        "Resources": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRuntimeVersionsResponseTypeDef = TypedDict(
     "DescribeRuntimeVersionsResponseTypeDef",
     {
         "RuntimeVersions": List[RuntimeVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociatedGroupsResponseTypeDef = TypedDict(
     "ListAssociatedGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CanaryTypeDef = TypedDict(
+    "CanaryTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Code": CanaryCodeOutputTypeDef,
+        "ExecutionRoleArn": str,
+        "Schedule": CanaryScheduleOutputTypeDef,
+        "RunConfig": CanaryRunConfigOutputTypeDef,
+        "SuccessRetentionPeriodInDays": int,
+        "FailureRetentionPeriodInDays": int,
+        "Status": CanaryStatusTypeDef,
+        "Timeline": CanaryTimelineTypeDef,
+        "ArtifactS3Location": str,
+        "EngineArn": str,
+        "RuntimeVersion": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "VisualReference": VisualReferenceOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ArtifactConfig": ArtifactConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateCanaryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCanaryRequestRequestTypeDef",
     {
         "Name": str,
         "Code": CanaryCodeInputTypeDef,
@@ -704,82 +752,58 @@
 
 class UpdateCanaryRequestRequestTypeDef(
     _RequiredUpdateCanaryRequestRequestTypeDef, _OptionalUpdateCanaryRequestRequestTypeDef
 ):
     pass
 
 
-CanaryTypeDef = TypedDict(
-    "CanaryTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Code": CanaryCodeOutputTypeDef,
-        "ExecutionRoleArn": str,
-        "Schedule": CanaryScheduleOutputTypeDef,
-        "RunConfig": CanaryRunConfigOutputTypeDef,
-        "SuccessRetentionPeriodInDays": int,
-        "FailureRetentionPeriodInDays": int,
-        "Status": CanaryStatusTypeDef,
-        "Timeline": CanaryTimelineTypeDef,
-        "ArtifactS3Location": str,
-        "EngineArn": str,
-        "RuntimeVersion": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "VisualReference": VisualReferenceOutputTypeDef,
-        "Tags": Dict[str, str],
-        "ArtifactConfig": ArtifactConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 CanaryLastRunTypeDef = TypedDict(
     "CanaryLastRunTypeDef",
     {
         "CanaryName": str,
         "LastRun": CanaryRunTypeDef,
     },
     total=False,
 )
 
 GetCanaryRunsResponseTypeDef = TypedDict(
     "GetCanaryRunsResponseTypeDef",
     {
         "CanaryRuns": List[CanaryRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCanaryResponseTypeDef = TypedDict(
     "CreateCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesResponseTypeDef = TypedDict(
     "DescribeCanariesResponseTypeDef",
     {
         "Canaries": List[CanaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCanaryResponseTypeDef = TypedDict(
     "GetCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesLastRunResponseTypeDef = TypedDict(
     "DescribeCanariesLastRunResponseTypeDef",
     {
         "CanariesLastRun": List[CanaryLastRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics/type_defs.pyi` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_synthetics.type_defs import S3EncryptionConfigTypeDef
 
-    data: S3EncryptionConfigTypeDef = {...}
+    data: S3EncryptionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -29,27 +29,29 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
     "AssociateResourceRequestRequestTypeDef",
+    "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
-    "CanaryCodeInputTypeDef",
+    "BlobTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
     "CanaryRunStatusTypeDef",
     "CanaryRunTimelineTypeDef",
     "CanaryScheduleInputTypeDef",
     "CanaryScheduleOutputTypeDef",
     "CanaryStatusTypeDef",
     "CanaryTimelineTypeDef",
     "VpcConfigOutputTypeDef",
     "VpcConfigInputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
     "DeleteCanaryRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DescribeCanariesLastRunRequestRequestTypeDef",
     "DescribeCanariesRequestRequestTypeDef",
     "DescribeRuntimeVersionsRequestRequestTypeDef",
@@ -57,36 +59,36 @@
     "DisassociateResourceRequestRequestTypeDef",
     "GetCanaryRequestRequestTypeDef",
     "GetCanaryRunsRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GroupSummaryTypeDef",
     "ListAssociatedGroupsRequestRequestTypeDef",
     "ListGroupResourcesRequestRequestTypeDef",
-    "ListGroupResourcesResponseTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartCanaryRequestRequestTypeDef",
     "StopCanaryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArtifactConfigInputTypeDef",
     "ArtifactConfigOutputTypeDef",
-    "VisualReferenceInputTypeDef",
     "VisualReferenceOutputTypeDef",
+    "VisualReferenceInputTypeDef",
+    "CanaryCodeInputTypeDef",
     "CanaryRunTypeDef",
+    "ListGroupResourcesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "DescribeRuntimeVersionsResponseTypeDef",
     "ListAssociatedGroupsResponseTypeDef",
     "ListGroupsResponseTypeDef",
+    "CanaryTypeDef",
     "CreateCanaryRequestRequestTypeDef",
     "UpdateCanaryRequestRequestTypeDef",
-    "CanaryTypeDef",
     "CanaryLastRunTypeDef",
     "GetCanaryRunsResponseTypeDef",
     "CreateCanaryResponseTypeDef",
     "DescribeCanariesResponseTypeDef",
     "GetCanaryResponseTypeDef",
     "DescribeCanariesLastRunResponseTypeDef",
 )
@@ -104,51 +106,51 @@
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
 
-_RequiredBaseScreenshotTypeDef = TypedDict(
-    "_RequiredBaseScreenshotTypeDef",
+_RequiredBaseScreenshotOutputTypeDef = TypedDict(
+    "_RequiredBaseScreenshotOutputTypeDef",
     {
         "ScreenshotName": str,
     },
 )
-_OptionalBaseScreenshotTypeDef = TypedDict(
-    "_OptionalBaseScreenshotTypeDef",
+_OptionalBaseScreenshotOutputTypeDef = TypedDict(
+    "_OptionalBaseScreenshotOutputTypeDef",
     {
         "IgnoreCoordinates": List[str],
     },
     total=False,
 )
 
-class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
+class BaseScreenshotOutputTypeDef(
+    _RequiredBaseScreenshotOutputTypeDef, _OptionalBaseScreenshotOutputTypeDef
+):
     pass
 
-_RequiredCanaryCodeInputTypeDef = TypedDict(
-    "_RequiredCanaryCodeInputTypeDef",
+_RequiredBaseScreenshotTypeDef = TypedDict(
+    "_RequiredBaseScreenshotTypeDef",
     {
-        "Handler": str,
+        "ScreenshotName": str,
     },
 )
-_OptionalCanaryCodeInputTypeDef = TypedDict(
-    "_OptionalCanaryCodeInputTypeDef",
+_OptionalBaseScreenshotTypeDef = TypedDict(
+    "_OptionalBaseScreenshotTypeDef",
     {
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3Version": str,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
+        "IgnoreCoordinates": Sequence[str],
     },
     total=False,
 )
 
-class CanaryCodeInputTypeDef(_RequiredCanaryCodeInputTypeDef, _OptionalCanaryCodeInputTypeDef):
+class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CanaryCodeOutputTypeDef = TypedDict(
     "CanaryCodeOutputTypeDef",
     {
         "SourceLocationArn": str,
         "Handler": str,
     },
     total=False,
@@ -258,14 +260,25 @@
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
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
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateGroupRequestRequestTypeDef = TypedDict(
@@ -450,23 +463,14 @@
 
 class ListGroupResourcesRequestRequestTypeDef(
     _RequiredListGroupResourcesRequestRequestTypeDef,
     _OptionalListGroupResourcesRequestRequestTypeDef,
 ):
     pass
 
-ListGroupResourcesResponseTypeDef = TypedDict(
-    "ListGroupResourcesResponseTypeDef",
-    {
-        "Resources": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -475,33 +479,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
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
 StartCanaryRequestRequestTypeDef = TypedDict(
     "StartCanaryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -540,14 +525,23 @@
     "ArtifactConfigOutputTypeDef",
     {
         "S3Encryption": S3EncryptionConfigTypeDef,
     },
     total=False,
 )
 
+VisualReferenceOutputTypeDef = TypedDict(
+    "VisualReferenceOutputTypeDef",
+    {
+        "BaseScreenshots": List[BaseScreenshotOutputTypeDef],
+        "BaseCanaryRunId": str,
+    },
+    total=False,
+)
+
 _RequiredVisualReferenceInputTypeDef = TypedDict(
     "_RequiredVisualReferenceInputTypeDef",
     {
         "BaseCanaryRunId": str,
     },
 )
 _OptionalVisualReferenceInputTypeDef = TypedDict(
@@ -559,78 +553,130 @@
 )
 
 class VisualReferenceInputTypeDef(
     _RequiredVisualReferenceInputTypeDef, _OptionalVisualReferenceInputTypeDef
 ):
     pass
 
-VisualReferenceOutputTypeDef = TypedDict(
-    "VisualReferenceOutputTypeDef",
+_RequiredCanaryCodeInputTypeDef = TypedDict(
+    "_RequiredCanaryCodeInputTypeDef",
     {
-        "BaseScreenshots": List[BaseScreenshotTypeDef],
-        "BaseCanaryRunId": str,
+        "Handler": str,
+    },
+)
+_OptionalCanaryCodeInputTypeDef = TypedDict(
+    "_OptionalCanaryCodeInputTypeDef",
+    {
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3Version": str,
+        "ZipFile": BlobTypeDef,
     },
     total=False,
 )
 
+class CanaryCodeInputTypeDef(_RequiredCanaryCodeInputTypeDef, _OptionalCanaryCodeInputTypeDef):
+    pass
+
 CanaryRunTypeDef = TypedDict(
     "CanaryRunTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": CanaryRunStatusTypeDef,
         "Timeline": CanaryRunTimelineTypeDef,
         "ArtifactS3Location": str,
     },
     total=False,
 )
 
+ListGroupResourcesResponseTypeDef = TypedDict(
+    "ListGroupResourcesResponseTypeDef",
+    {
+        "Resources": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRuntimeVersionsResponseTypeDef = TypedDict(
     "DescribeRuntimeVersionsResponseTypeDef",
     {
         "RuntimeVersions": List[RuntimeVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociatedGroupsResponseTypeDef = TypedDict(
     "ListAssociatedGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CanaryTypeDef = TypedDict(
+    "CanaryTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Code": CanaryCodeOutputTypeDef,
+        "ExecutionRoleArn": str,
+        "Schedule": CanaryScheduleOutputTypeDef,
+        "RunConfig": CanaryRunConfigOutputTypeDef,
+        "SuccessRetentionPeriodInDays": int,
+        "FailureRetentionPeriodInDays": int,
+        "Status": CanaryStatusTypeDef,
+        "Timeline": CanaryTimelineTypeDef,
+        "ArtifactS3Location": str,
+        "EngineArn": str,
+        "RuntimeVersion": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "VisualReference": VisualReferenceOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ArtifactConfig": ArtifactConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateCanaryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCanaryRequestRequestTypeDef",
     {
         "Name": str,
         "Code": CanaryCodeInputTypeDef,
         "ArtifactS3Location": str,
         "ExecutionRoleArn": str,
@@ -681,82 +727,58 @@
 )
 
 class UpdateCanaryRequestRequestTypeDef(
     _RequiredUpdateCanaryRequestRequestTypeDef, _OptionalUpdateCanaryRequestRequestTypeDef
 ):
     pass
 
-CanaryTypeDef = TypedDict(
-    "CanaryTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Code": CanaryCodeOutputTypeDef,
-        "ExecutionRoleArn": str,
-        "Schedule": CanaryScheduleOutputTypeDef,
-        "RunConfig": CanaryRunConfigOutputTypeDef,
-        "SuccessRetentionPeriodInDays": int,
-        "FailureRetentionPeriodInDays": int,
-        "Status": CanaryStatusTypeDef,
-        "Timeline": CanaryTimelineTypeDef,
-        "ArtifactS3Location": str,
-        "EngineArn": str,
-        "RuntimeVersion": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "VisualReference": VisualReferenceOutputTypeDef,
-        "Tags": Dict[str, str],
-        "ArtifactConfig": ArtifactConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 CanaryLastRunTypeDef = TypedDict(
     "CanaryLastRunTypeDef",
     {
         "CanaryName": str,
         "LastRun": CanaryRunTypeDef,
     },
     total=False,
 )
 
 GetCanaryRunsResponseTypeDef = TypedDict(
     "GetCanaryRunsResponseTypeDef",
     {
         "CanaryRuns": List[CanaryRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCanaryResponseTypeDef = TypedDict(
     "CreateCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesResponseTypeDef = TypedDict(
     "DescribeCanariesResponseTypeDef",
     {
         "Canaries": List[CanaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCanaryResponseTypeDef = TypedDict(
     "GetCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesLastRunResponseTypeDef = TypedDict(
     "DescribeCanariesLastRunResponseTypeDef",
     {
         "CanariesLastRun": List[CanaryLastRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/PKG-INFO` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-synthetics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore synthetics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore synthetics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-synthetics"></a>
 
 # types-aiobotocore-synthetics
 
 [![PyPI - types-aiobotocore-synthetics](https://img.shields.io/pypi/v/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-synthetics?color=blue)](https://pypistats.org/packages/types-aiobotocore-synthetics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-synthetics)](https://pepy.tech/project/types-aiobotocore-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Synthetics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
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
@@ -285,38 +284,40 @@
 )
 
 
 def check_value(value: CanaryRunStateReasonCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_synthetics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
-    CanaryCodeInputTypeDef,
+    BlobTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
     CanaryRunStatusTypeDef,
     CanaryRunTimelineTypeDef,
     CanaryScheduleInputTypeDef,
     CanaryScheduleOutputTypeDef,
     CanaryStatusTypeDef,
     CanaryTimelineTypeDef,
     VpcConfigOutputTypeDef,
     VpcConfigInputTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     DeleteCanaryRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DescribeCanariesLastRunRequestRequestTypeDef,
     DescribeCanariesRequestRequestTypeDef,
     DescribeRuntimeVersionsRequestRequestTypeDef,
@@ -324,46 +325,46 @@
     DisassociateResourceRequestRequestTypeDef,
     GetCanaryRequestRequestTypeDef,
     GetCanaryRunsRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GroupSummaryTypeDef,
     ListAssociatedGroupsRequestRequestTypeDef,
     ListGroupResourcesRequestRequestTypeDef,
-    ListGroupResourcesResponseTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartCanaryRequestRequestTypeDef,
     StopCanaryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArtifactConfigInputTypeDef,
     ArtifactConfigOutputTypeDef,
-    VisualReferenceInputTypeDef,
     VisualReferenceOutputTypeDef,
+    VisualReferenceInputTypeDef,
+    CanaryCodeInputTypeDef,
     CanaryRunTypeDef,
+    ListGroupResourcesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     DescribeRuntimeVersionsResponseTypeDef,
     ListAssociatedGroupsResponseTypeDef,
     ListGroupsResponseTypeDef,
+    CanaryTypeDef,
     CreateCanaryRequestRequestTypeDef,
     UpdateCanaryRequestRequestTypeDef,
-    CanaryTypeDef,
     CanaryLastRunTypeDef,
     GetCanaryRunsResponseTypeDef,
     CreateCanaryResponseTypeDef,
     DescribeCanariesResponseTypeDef,
     GetCanaryResponseTypeDef,
     DescribeCanariesLastRunResponseTypeDef,
 )
 
 
-def get_structure() -> S3EncryptionConfigTypeDef:
+def get_value() -> S3EncryptionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-synthetics-2.5.2/types_aiobotocore_synthetics.egg-info/SOURCES.txt` & `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


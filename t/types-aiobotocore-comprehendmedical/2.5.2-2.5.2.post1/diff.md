# Comparing `tmp/types-aiobotocore-comprehendmedical-2.5.2.tar.gz` & `tmp/types-aiobotocore-comprehendmedical-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehendmedical-2.5.2.tar", last modified: Sat Jul  8 01:43:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehendmedical-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
```

## Comparing `types-aiobotocore-comprehendmedical-2.5.2.tar` & `types-aiobotocore-comprehendmedical-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.221915 types-aiobotocore-comprehendmedical-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16055 2023-07-08 01:43:26.221915 types-aiobotocore-comprehendmedical-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:26.221915 types-aiobotocore-comprehendmedical-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.217914 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-08 01:27:56.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-07-08 01:27:56.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-07-08 01:27:57.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24947 2023-07-08 01:27:56.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:55.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.217914 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16055 2023-07-08 01:43:26.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:43:26.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:26.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:26.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:26.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:26.000000 types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-08-02 14:35:32.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/LICENSE` & `types-aiobotocore-comprehendmedical-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/PKG-INFO` & `types-aiobotocore-comprehendmedical-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehendmedical
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore comprehendmedical type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-comprehendmedical"></a>
 
 # types-aiobotocore-comprehendmedical
 
 [![PyPI - types-aiobotocore-comprehendmedical](https://img.shields.io/pypi/v/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-comprehendmedical?color=blue)](https://pypistats.org/packages/types-aiobotocore-comprehendmedical)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ComprehendMedical 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [types-aiobotocore-comprehendmedical docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/).
 
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
@@ -300,79 +299,80 @@
 )
 
 
 def check_value(value: AttributeNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_comprehendmedical.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
-    ComprehendMedicalAsyncJobFilterTypeDef,
+    TimestampTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
-    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
-    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
-    ListICD10CMInferenceJobsRequestRequestTypeDef,
-    ListPHIDetectionJobsRequestRequestTypeDef,
-    ListRxNormInferenceJobsRequestRequestTypeDef,
-    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
+    ComprehendMedicalAsyncJobFilterTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
+    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
+    ListICD10CMInferenceJobsRequestRequestTypeDef,
+    ListPHIDetectionJobsRequestRequestTypeDef,
+    ListRxNormInferenceJobsRequestRequestTypeDef,
+    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
     DescribeRxNormInferenceJobResponseTypeDef,
     DescribeSNOMEDCTInferenceJobResponseTypeDef,
     ListEntitiesDetectionV2JobsResponseTypeDef,
     ListICD10CMInferenceJobsResponseTypeDef,
@@ -387,15 +387,15 @@
     DetectEntitiesV2ResponseTypeDef,
     InferICD10CMResponseTypeDef,
     InferRxNormResponseTypeDef,
     InferSNOMEDCTResponseTypeDef,
 )
 
 
-def get_structure() -> TraitTypeDef:
+def get_value() -> TraitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/README.md` & `types-aiobotocore-comprehendmedical-2.5.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-comprehendmedical"></a>
 
 # types-aiobotocore-comprehendmedical
 
 [![PyPI - types-aiobotocore-comprehendmedical](https://img.shields.io/pypi/v/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-comprehendmedical?color=blue)](https://pypistats.org/packages/types-aiobotocore-comprehendmedical)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ComprehendMedical 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [types-aiobotocore-comprehendmedical docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/).
 
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
@@ -267,79 +267,80 @@
 )
 
 
 def check_value(value: AttributeNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_comprehendmedical.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
-    ComprehendMedicalAsyncJobFilterTypeDef,
+    TimestampTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
-    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
-    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
-    ListICD10CMInferenceJobsRequestRequestTypeDef,
-    ListPHIDetectionJobsRequestRequestTypeDef,
-    ListRxNormInferenceJobsRequestRequestTypeDef,
-    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
+    ComprehendMedicalAsyncJobFilterTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
+    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
+    ListICD10CMInferenceJobsRequestRequestTypeDef,
+    ListPHIDetectionJobsRequestRequestTypeDef,
+    ListRxNormInferenceJobsRequestRequestTypeDef,
+    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
     DescribeRxNormInferenceJobResponseTypeDef,
     DescribeSNOMEDCTInferenceJobResponseTypeDef,
     ListEntitiesDetectionV2JobsResponseTypeDef,
     ListICD10CMInferenceJobsResponseTypeDef,
@@ -354,15 +355,15 @@
     DetectEntitiesV2ResponseTypeDef,
     InferICD10CMResponseTypeDef,
     InferRxNormResponseTypeDef,
     InferSNOMEDCTResponseTypeDef,
 )
 
 
-def get_structure() -> TraitTypeDef:
+def get_value() -> TraitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/setup.py` & `types-aiobotocore-comprehendmedical-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehendmedical",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with"
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
-        "aiobotocore comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore comprehendmedical type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_comprehendmedical": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/"
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/__init__.py` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/__init__.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/__main__.py` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ComprehendMedical 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ComprehendMedical 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
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

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/client.py` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/client.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/literals.py` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/literals.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/type_defs.py` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_comprehendmedical.type_defs import TraitTypeDef
 
-    data: TraitTypeDef = {...}
+    data: TraitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Union
 
 from .literals import (
@@ -44,68 +44,69 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
-    "ComprehendMedicalAsyncJobFilterTypeDef",
+    "TimestampTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    "StartICD10CMInferenceJobResponseTypeDef",
-    "StartPHIDetectionJobResponseTypeDef",
-    "StartRxNormInferenceJobResponseTypeDef",
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
-    "StopEntitiesDetectionV2JobResponseTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
-    "StopICD10CMInferenceJobResponseTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
-    "StopPHIDetectionJobResponseTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
-    "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "AttributeTypeDef",
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    "StartICD10CMInferenceJobResponseTypeDef",
+    "StartPHIDetectionJobResponseTypeDef",
+    "StartRxNormInferenceJobResponseTypeDef",
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    "StopICD10CMInferenceJobResponseTypeDef",
+    "StopPHIDetectionJobResponseTypeDef",
+    "StopRxNormInferenceJobResponseTypeDef",
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
     "DescribeRxNormInferenceJobResponseTypeDef",
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     "ListICD10CMInferenceJobsResponseTypeDef",
@@ -136,25 +137,15 @@
     "CharactersTypeDef",
     {
         "OriginalTextCharacters": int,
     },
     total=False,
 )
 
-ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
-    "ComprehendMedicalAsyncJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
@@ -192,14 +183,25 @@
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
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
 DescribeICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -291,25 +293,14 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
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
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
         "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
@@ -340,129 +331,49 @@
     {
         "Name": SNOMEDCTTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
-StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StartICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartPHIDetectionJobResponseTypeDef = TypedDict(
-    "StartPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StartRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StopICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "StopPHIDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopPHIDetectionJobResponseTypeDef = TypedDict(
-    "StopPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "StopRxNormInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StopRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Type": EntitySubTypeType,
         "Score": float,
         "RelationshipScore": float,
         "RelationshipType": RelationshipTypeType,
@@ -472,60 +383,21 @@
         "Text": str,
         "Category": EntityTypeType,
         "Traits": List[TraitTypeDef],
     },
     total=False,
 )
 
-ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ComprehendMedicalAsyncJobPropertiesTypeDef = TypedDict(
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     {
@@ -678,14 +550,94 @@
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
 
+StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StartICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPHIDetectionJobResponseTypeDef = TypedDict(
+    "StartPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StartRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StopICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPHIDetectionJobResponseTypeDef = TypedDict(
+    "StopPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StopRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ICD10CMAttributeTypeDef = TypedDict(
     "ICD10CMAttributeTypeDef",
     {
         "Type": ICD10CMAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
@@ -753,96 +705,146 @@
     {
         "Type": EntityTypeType,
         "Attribute": AttributeTypeDef,
     },
     total=False,
 )
 
+ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeICD10CMInferenceJobResponseTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePHIDetectionJobResponseTypeDef = TypedDict(
     "DescribePHIDetectionJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRxNormInferenceJobResponseTypeDef = TypedDict(
     "DescribeRxNormInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionV2JobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListICD10CMInferenceJobsResponseTypeDef = TypedDict(
     "ListICD10CMInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPHIDetectionJobsResponseTypeDef = TypedDict(
     "ListPHIDetectionJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRxNormInferenceJobsResponseTypeDef = TypedDict(
     "ListRxNormInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSNOMEDCTInferenceJobsResponseTypeDef = TypedDict(
     "ListSNOMEDCTInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ICD10CMEntityTypeDef = TypedDict(
     "ICD10CMEntityTypeDef",
     {
         "Id": int,
@@ -895,64 +897,64 @@
 
 DetectPHIResponseTypeDef = TypedDict(
     "DetectPHIResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesResponseTypeDef = TypedDict(
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesV2ResponseTypeDef = TypedDict(
     "DetectEntitiesV2ResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferICD10CMResponseTypeDef = TypedDict(
     "InferICD10CMResponseTypeDef",
     {
         "Entities": List[ICD10CMEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferRxNormResponseTypeDef = TypedDict(
     "InferRxNormResponseTypeDef",
     {
         "Entities": List[RxNormEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferSNOMEDCTResponseTypeDef = TypedDict(
     "InferSNOMEDCTResponseTypeDef",
     {
         "Entities": List[SNOMEDCTEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
         "SNOMEDCTDetails": SNOMEDCTDetailsTypeDef,
         "Characters": CharactersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical/type_defs.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_comprehendmedical.type_defs import TraitTypeDef
 
-    data: TraitTypeDef = {...}
+    data: TraitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Union
 
 from .literals import (
@@ -43,68 +43,69 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
-    "ComprehendMedicalAsyncJobFilterTypeDef",
+    "TimestampTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    "StartICD10CMInferenceJobResponseTypeDef",
-    "StartPHIDetectionJobResponseTypeDef",
-    "StartRxNormInferenceJobResponseTypeDef",
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
-    "StopEntitiesDetectionV2JobResponseTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
-    "StopICD10CMInferenceJobResponseTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
-    "StopPHIDetectionJobResponseTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
-    "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "AttributeTypeDef",
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    "StartICD10CMInferenceJobResponseTypeDef",
+    "StartPHIDetectionJobResponseTypeDef",
+    "StartRxNormInferenceJobResponseTypeDef",
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    "StopICD10CMInferenceJobResponseTypeDef",
+    "StopPHIDetectionJobResponseTypeDef",
+    "StopRxNormInferenceJobResponseTypeDef",
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
     "DescribeRxNormInferenceJobResponseTypeDef",
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     "ListICD10CMInferenceJobsResponseTypeDef",
@@ -135,25 +136,15 @@
     "CharactersTypeDef",
     {
         "OriginalTextCharacters": int,
     },
     total=False,
 )
 
-ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
-    "ComprehendMedicalAsyncJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
@@ -187,14 +178,25 @@
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
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
 DescribeICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -286,25 +288,14 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
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
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
         "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
@@ -335,129 +326,49 @@
     {
         "Name": SNOMEDCTTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
-StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StartICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartPHIDetectionJobResponseTypeDef = TypedDict(
-    "StartPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StartRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StopICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "StopPHIDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopPHIDetectionJobResponseTypeDef = TypedDict(
-    "StopPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "StopRxNormInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StopRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Type": EntitySubTypeType,
         "Score": float,
         "RelationshipScore": float,
         "RelationshipType": RelationshipTypeType,
@@ -467,60 +378,21 @@
         "Text": str,
         "Category": EntityTypeType,
         "Traits": List[TraitTypeDef],
     },
     total=False,
 )
 
-ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ComprehendMedicalAsyncJobPropertiesTypeDef = TypedDict(
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     {
@@ -663,14 +535,94 @@
 
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
+StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StartICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPHIDetectionJobResponseTypeDef = TypedDict(
+    "StartPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StartRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StopICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPHIDetectionJobResponseTypeDef = TypedDict(
+    "StopPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StopRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ICD10CMAttributeTypeDef = TypedDict(
     "ICD10CMAttributeTypeDef",
     {
         "Type": ICD10CMAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
@@ -738,96 +690,146 @@
     {
         "Type": EntityTypeType,
         "Attribute": AttributeTypeDef,
     },
     total=False,
 )
 
+ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeICD10CMInferenceJobResponseTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePHIDetectionJobResponseTypeDef = TypedDict(
     "DescribePHIDetectionJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRxNormInferenceJobResponseTypeDef = TypedDict(
     "DescribeRxNormInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionV2JobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListICD10CMInferenceJobsResponseTypeDef = TypedDict(
     "ListICD10CMInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPHIDetectionJobsResponseTypeDef = TypedDict(
     "ListPHIDetectionJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRxNormInferenceJobsResponseTypeDef = TypedDict(
     "ListRxNormInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSNOMEDCTInferenceJobsResponseTypeDef = TypedDict(
     "ListSNOMEDCTInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ICD10CMEntityTypeDef = TypedDict(
     "ICD10CMEntityTypeDef",
     {
         "Id": int,
@@ -880,64 +882,64 @@
 
 DetectPHIResponseTypeDef = TypedDict(
     "DetectPHIResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesResponseTypeDef = TypedDict(
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesV2ResponseTypeDef = TypedDict(
     "DetectEntitiesV2ResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferICD10CMResponseTypeDef = TypedDict(
     "InferICD10CMResponseTypeDef",
     {
         "Entities": List[ICD10CMEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferRxNormResponseTypeDef = TypedDict(
     "InferRxNormResponseTypeDef",
     {
         "Entities": List[RxNormEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferSNOMEDCTResponseTypeDef = TypedDict(
     "InferSNOMEDCTResponseTypeDef",
     {
         "Entities": List[SNOMEDCTEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
         "SNOMEDCTDetails": SNOMEDCTDetailsTypeDef,
         "Characters": CharactersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehendmedical
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore comprehendmedical type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-comprehendmedical"></a>
 
 # types-aiobotocore-comprehendmedical
 
 [![PyPI - types-aiobotocore-comprehendmedical](https://img.shields.io/pypi/v/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-comprehendmedical?color=blue)](https://pypistats.org/packages/types-aiobotocore-comprehendmedical)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ComprehendMedical 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [types-aiobotocore-comprehendmedical docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/).
 
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
@@ -300,79 +299,80 @@
 )
 
 
 def check_value(value: AttributeNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_comprehendmedical.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
-    ComprehendMedicalAsyncJobFilterTypeDef,
+    TimestampTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
-    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
-    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
-    ListICD10CMInferenceJobsRequestRequestTypeDef,
-    ListPHIDetectionJobsRequestRequestTypeDef,
-    ListRxNormInferenceJobsRequestRequestTypeDef,
-    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
+    ComprehendMedicalAsyncJobFilterTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
+    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
+    ListICD10CMInferenceJobsRequestRequestTypeDef,
+    ListPHIDetectionJobsRequestRequestTypeDef,
+    ListRxNormInferenceJobsRequestRequestTypeDef,
+    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
     DescribeRxNormInferenceJobResponseTypeDef,
     DescribeSNOMEDCTInferenceJobResponseTypeDef,
     ListEntitiesDetectionV2JobsResponseTypeDef,
     ListICD10CMInferenceJobsResponseTypeDef,
@@ -387,15 +387,15 @@
     DetectEntitiesV2ResponseTypeDef,
     InferICD10CMResponseTypeDef,
     InferRxNormResponseTypeDef,
     InferSNOMEDCTResponseTypeDef,
 )
 
 
-def get_structure() -> TraitTypeDef:
+def get_value() -> TraitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt` & `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-dlm-2.5.2.tar.gz` & `tmp/types-aiobotocore-dlm-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dlm-2.5.2.tar", last modified: Sat Jul  8 01:43:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-dlm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:11 2023, max compression
```

## Comparing `types-aiobotocore-dlm-2.5.2.tar` & `types-aiobotocore-dlm-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:31.698019 types-aiobotocore-dlm-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-08 01:43:31.698019 types-aiobotocore-dlm-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:31.698019 types-aiobotocore-dlm-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:31.698019 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-08 01:28:49.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-08 01:28:49.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-07-08 01:28:50.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-07-08 01:28:49.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:48.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:31.698019 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-08 01:43:31.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-08 01:43:31.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:31.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:31.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:31.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:31.000000 types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.697602 types-aiobotocore-dlm-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-08-02 14:52:11.685602 types-aiobotocore-dlm-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:11.697602 types-aiobotocore-dlm-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.685602 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-08-02 14:36:29.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-08-02 14:36:29.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.685602 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dlm-2.5.2/LICENSE` & `types-aiobotocore-dlm-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2/PKG-INFO` & `types-aiobotocore-dlm-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dlm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dlm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dlm"></a>
 
 # types-aiobotocore-dlm
 
 [![PyPI - types-aiobotocore-dlm](https://img.shields.io/pypi/v/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dlm?color=blue)](https://pypistats.org/packages/types-aiobotocore-dlm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DLM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
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
@@ -288,62 +287,72 @@
 )
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dlm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
+    CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
     DeprecateRuleTypeDef,
+    EventParametersOutputTypeDef,
     EventParametersTypeDef,
+    FastRestoreRuleOutputTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     RetainRuleTypeDef,
+    ShareRuleOutputTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArchiveRetainRuleTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
     CrossRegionCopyRuleTypeDef,
+    EventSourceOutputTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
+    ParametersOutputTypeDef,
     ParametersTypeDef,
     ArchiveRuleTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ScheduleOutputTypeDef,
     ScheduleTypeDef,
+    PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
-    CreateLifecyclePolicyRequestRequestTypeDef,
     LifecyclePolicyTypeDef,
+    CreateLifecyclePolicyRequestRequestTypeDef,
+    PolicyDetailsUnionTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierTypeDef:
+def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dlm-2.5.2/README.md` & `types-aiobotocore-dlm-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-dlm"></a>
 
 # types-aiobotocore-dlm
 
 [![PyPI - types-aiobotocore-dlm](https://img.shields.io/pypi/v/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dlm?color=blue)](https://pypistats.org/packages/types-aiobotocore-dlm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DLM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
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
@@ -255,62 +255,72 @@
 )
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dlm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
+    CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
     DeprecateRuleTypeDef,
+    EventParametersOutputTypeDef,
     EventParametersTypeDef,
+    FastRestoreRuleOutputTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     RetainRuleTypeDef,
+    ShareRuleOutputTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArchiveRetainRuleTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
     CrossRegionCopyRuleTypeDef,
+    EventSourceOutputTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
+    ParametersOutputTypeDef,
     ParametersTypeDef,
     ArchiveRuleTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ScheduleOutputTypeDef,
     ScheduleTypeDef,
+    PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
-    CreateLifecyclePolicyRequestRequestTypeDef,
     LifecyclePolicyTypeDef,
+    CreateLifecyclePolicyRequestRequestTypeDef,
+    PolicyDetailsUnionTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierTypeDef:
+def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dlm-2.5.2/setup.py` & `types-aiobotocore-dlm-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dlm",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore dlm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore dlm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dlm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/__main__.py` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DLM 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DLM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/client.py` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyDetailsTypeDef,
+    PolicyDetailsUnionTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -86,15 +86,15 @@
 
     async def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: PolicyDetailsTypeDef,
+        PolicyDetails: PolicyDetailsUnionTypeDef,
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -177,15 +177,15 @@
     async def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: PolicyDetailsTypeDef = ...
+        PolicyDetails: PolicyDetailsUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/client.pyi` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyDetailsTypeDef,
+    PolicyDetailsUnionTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -80,15 +80,15 @@
         """
     async def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: PolicyDetailsTypeDef,
+        PolicyDetails: PolicyDetailsUnionTypeDef,
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -163,15 +163,15 @@
     async def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: PolicyDetailsTypeDef = ...
+        PolicyDetails: PolicyDetailsUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/literals.py` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/literals.pyi` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm/type_defs.pyi` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/type_defs.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dlm.type_defs import RetentionArchiveTierTypeDef
 
-    data: RetentionArchiveTierTypeDef = {...}
+    data: RetentionArchiveTierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GettablePolicyStateValuesType,
     LocationValuesType,
     PolicyTypeValuesType,
     ResourceLocationValuesType,
     ResourceTypeValuesType,
@@ -32,68 +32,93 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "RetentionArchiveTierTypeDef",
-    "CreateLifecyclePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "CreateRuleOutputTypeDef",
     "CreateRuleTypeDef",
     "CrossRegionCopyRetainRuleTypeDef",
     "EncryptionConfigurationTypeDef",
     "CrossRegionCopyDeprecateRuleTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
     "DeprecateRuleTypeDef",
+    "EventParametersOutputTypeDef",
     "EventParametersTypeDef",
+    "FastRestoreRuleOutputTypeDef",
     "FastRestoreRuleTypeDef",
     "GetLifecyclePoliciesRequestRequestTypeDef",
     "LifecyclePolicySummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "RetainRuleTypeDef",
+    "ShareRuleOutputTypeDef",
     "ShareRuleTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArchiveRetainRuleTypeDef",
+    "CreateLifecyclePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CrossRegionCopyActionTypeDef",
     "CrossRegionCopyRuleTypeDef",
+    "EventSourceOutputTypeDef",
     "EventSourceTypeDef",
     "GetLifecyclePoliciesResponseTypeDef",
+    "ParametersOutputTypeDef",
     "ParametersTypeDef",
     "ArchiveRuleTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
+    "PolicyDetailsOutputTypeDef",
     "PolicyDetailsTypeDef",
-    "CreateLifecyclePolicyRequestRequestTypeDef",
     "LifecyclePolicyTypeDef",
+    "CreateLifecyclePolicyRequestRequestTypeDef",
+    "PolicyDetailsUnionTypeDef",
     "UpdateLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
 )
 
 RetentionArchiveTierTypeDef = TypedDict(
     "RetentionArchiveTierTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
-CreateLifecyclePolicyResponseTypeDef = TypedDict(
-    "CreateLifecyclePolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PolicyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
+    {
+        "Location": LocationValuesType,
+        "Interval": int,
+        "IntervalUnit": Literal["HOURS"],
+        "Times": List[str],
+        "CronExpression": str,
+    },
+    total=False,
+)
+
 CreateRuleTypeDef = TypedDict(
     "CreateRuleTypeDef",
     {
         "Location": LocationValuesType,
         "Interval": int,
         "IntervalUnit": Literal["HOURS"],
         "Times": Sequence[str],
@@ -152,23 +177,53 @@
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
+EventParametersOutputTypeDef = TypedDict(
+    "EventParametersOutputTypeDef",
+    {
+        "EventType": Literal["shareSnapshot"],
+        "SnapshotOwner": List[str],
+        "DescriptionRegex": str,
+    },
+)
+
 EventParametersTypeDef = TypedDict(
     "EventParametersTypeDef",
     {
         "EventType": Literal["shareSnapshot"],
         "SnapshotOwner": Sequence[str],
         "DescriptionRegex": str,
     },
 )
 
+_RequiredFastRestoreRuleOutputTypeDef = TypedDict(
+    "_RequiredFastRestoreRuleOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+    },
+)
+_OptionalFastRestoreRuleOutputTypeDef = TypedDict(
+    "_OptionalFastRestoreRuleOutputTypeDef",
+    {
+        "Count": int,
+        "Interval": int,
+        "IntervalUnit": RetentionIntervalUnitValuesType,
+    },
+    total=False,
+)
+
+class FastRestoreRuleOutputTypeDef(
+    _RequiredFastRestoreRuleOutputTypeDef, _OptionalFastRestoreRuleOutputTypeDef
+):
+    pass
+
 _RequiredFastRestoreRuleTypeDef = TypedDict(
     "_RequiredFastRestoreRuleTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
 )
 _OptionalFastRestoreRuleTypeDef = TypedDict(
@@ -218,51 +273,50 @@
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 RetainRuleTypeDef = TypedDict(
     "RetainRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
+_RequiredShareRuleOutputTypeDef = TypedDict(
+    "_RequiredShareRuleOutputTypeDef",
+    {
+        "TargetAccounts": List[str],
+    },
+)
+_OptionalShareRuleOutputTypeDef = TypedDict(
+    "_OptionalShareRuleOutputTypeDef",
+    {
+        "UnshareInterval": int,
+        "UnshareIntervalUnit": RetentionIntervalUnitValuesType,
+    },
+    total=False,
+)
+
+class ShareRuleOutputTypeDef(_RequiredShareRuleOutputTypeDef, _OptionalShareRuleOutputTypeDef):
+    pass
+
 _RequiredShareRuleTypeDef = TypedDict(
     "_RequiredShareRuleTypeDef",
     {
         "TargetAccounts": Sequence[str],
     },
 )
 _OptionalShareRuleTypeDef = TypedDict(
@@ -296,14 +350,30 @@
 ArchiveRetainRuleTypeDef = TypedDict(
     "ArchiveRetainRuleTypeDef",
     {
         "RetentionArchiveTier": RetentionArchiveTierTypeDef,
     },
 )
 
+CreateLifecyclePolicyResponseTypeDef = TypedDict(
+    "CreateLifecyclePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
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
 _RequiredCrossRegionCopyActionTypeDef = TypedDict(
     "_RequiredCrossRegionCopyActionTypeDef",
     {
         "Target": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
@@ -340,14 +410,33 @@
 )
 
 class CrossRegionCopyRuleTypeDef(
     _RequiredCrossRegionCopyRuleTypeDef, _OptionalCrossRegionCopyRuleTypeDef
 ):
     pass
 
+_RequiredEventSourceOutputTypeDef = TypedDict(
+    "_RequiredEventSourceOutputTypeDef",
+    {
+        "Type": Literal["MANAGED_CWE"],
+    },
+)
+_OptionalEventSourceOutputTypeDef = TypedDict(
+    "_OptionalEventSourceOutputTypeDef",
+    {
+        "Parameters": EventParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+class EventSourceOutputTypeDef(
+    _RequiredEventSourceOutputTypeDef, _OptionalEventSourceOutputTypeDef
+):
+    pass
+
 _RequiredEventSourceTypeDef = TypedDict(
     "_RequiredEventSourceTypeDef",
     {
         "Type": Literal["MANAGED_CWE"],
     },
 )
 _OptionalEventSourceTypeDef = TypedDict(
@@ -361,18 +450,28 @@
 class EventSourceTypeDef(_RequiredEventSourceTypeDef, _OptionalEventSourceTypeDef):
     pass
 
 GetLifecyclePoliciesResponseTypeDef = TypedDict(
     "GetLifecyclePoliciesResponseTypeDef",
     {
         "Policies": List[LifecyclePolicySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ParametersOutputTypeDef = TypedDict(
+    "ParametersOutputTypeDef",
+    {
+        "ExcludeBootVolume": bool,
+        "NoReboot": bool,
+        "ExcludeDataVolumeTags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 ParametersTypeDef = TypedDict(
     "ParametersTypeDef",
     {
         "ExcludeBootVolume": bool,
         "NoReboot": bool,
         "ExcludeDataVolumeTags": Sequence[TagTypeDef],
     },
@@ -382,22 +481,48 @@
 ArchiveRuleTypeDef = TypedDict(
     "ArchiveRuleTypeDef",
     {
         "RetainRule": ArchiveRetainRuleTypeDef,
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "Name": str,
+        "CrossRegionCopy": List[CrossRegionCopyActionTypeDef],
+    },
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
         "CrossRegionCopy": Sequence[CrossRegionCopyActionTypeDef],
     },
 )
 
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "Name": str,
+        "CopyTags": bool,
+        "TagsToAdd": List[TagTypeDef],
+        "VariableTags": List[TagTypeDef],
+        "CreateRule": CreateRuleOutputTypeDef,
+        "RetainRule": RetainRuleTypeDef,
+        "FastRestoreRule": FastRestoreRuleOutputTypeDef,
+        "CrossRegionCopyRules": List[CrossRegionCopyRuleTypeDef],
+        "ShareRules": List[ShareRuleOutputTypeDef],
+        "DeprecateRule": DeprecateRuleTypeDef,
+        "ArchiveRule": ArchiveRuleTypeDef,
+    },
+    total=False,
+)
+
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "Name": str,
         "CopyTags": bool,
         "TagsToAdd": Sequence[TagTypeDef],
         "VariableTags": Sequence[TagTypeDef],
@@ -408,14 +533,29 @@
         "ShareRules": Sequence[ShareRuleTypeDef],
         "DeprecateRule": DeprecateRuleTypeDef,
         "ArchiveRule": ArchiveRuleTypeDef,
     },
     total=False,
 )
 
+PolicyDetailsOutputTypeDef = TypedDict(
+    "PolicyDetailsOutputTypeDef",
+    {
+        "PolicyType": PolicyTypeValuesType,
+        "ResourceTypes": List[ResourceTypeValuesType],
+        "ResourceLocations": List[ResourceLocationValuesType],
+        "TargetTags": List[TagTypeDef],
+        "Schedules": List[ScheduleOutputTypeDef],
+        "Parameters": ParametersOutputTypeDef,
+        "EventSource": EventSourceOutputTypeDef,
+        "Actions": List[ActionOutputTypeDef],
+    },
+    total=False,
+)
+
 PolicyDetailsTypeDef = TypedDict(
     "PolicyDetailsTypeDef",
     {
         "PolicyType": PolicyTypeValuesType,
         "ResourceTypes": Sequence[ResourceTypeValuesType],
         "ResourceLocations": Sequence[ResourceLocationValuesType],
         "TargetTags": Sequence[TagTypeDef],
@@ -423,14 +563,31 @@
         "Parameters": ParametersTypeDef,
         "EventSource": EventSourceTypeDef,
         "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
+LifecyclePolicyTypeDef = TypedDict(
+    "LifecyclePolicyTypeDef",
+    {
+        "PolicyId": str,
+        "Description": str,
+        "State": GettablePolicyStateValuesType,
+        "StatusMessage": str,
+        "ExecutionRoleArn": str,
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "PolicyDetails": PolicyDetailsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "PolicyArn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLifecyclePolicyRequestRequestTypeDef",
     {
         "ExecutionRoleArn": str,
         "Description": str,
         "State": SettablePolicyStateValuesType,
         "PolicyDetails": PolicyDetailsTypeDef,
@@ -446,31 +603,15 @@
 
 class CreateLifecyclePolicyRequestRequestTypeDef(
     _RequiredCreateLifecyclePolicyRequestRequestTypeDef,
     _OptionalCreateLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-LifecyclePolicyTypeDef = TypedDict(
-    "LifecyclePolicyTypeDef",
-    {
-        "PolicyId": str,
-        "Description": str,
-        "State": GettablePolicyStateValuesType,
-        "StatusMessage": str,
-        "ExecutionRoleArn": str,
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "PolicyDetails": PolicyDetailsTypeDef,
-        "Tags": Dict[str, str],
-        "PolicyArn": str,
-    },
-    total=False,
-)
-
+PolicyDetailsUnionTypeDef = Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef]
 _RequiredUpdateLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLifecyclePolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalUpdateLifecyclePolicyRequestRequestTypeDef = TypedDict(
@@ -490,10 +631,10 @@
 ):
     pass
 
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "Policy": LifecyclePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/PKG-INFO` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dlm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dlm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dlm"></a>
 
 # types-aiobotocore-dlm
 
 [![PyPI - types-aiobotocore-dlm](https://img.shields.io/pypi/v/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dlm?color=blue)](https://pypistats.org/packages/types-aiobotocore-dlm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DLM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
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
@@ -288,62 +287,72 @@
 )
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dlm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
+    CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
     DeprecateRuleTypeDef,
+    EventParametersOutputTypeDef,
     EventParametersTypeDef,
+    FastRestoreRuleOutputTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     RetainRuleTypeDef,
+    ShareRuleOutputTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArchiveRetainRuleTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
     CrossRegionCopyRuleTypeDef,
+    EventSourceOutputTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
+    ParametersOutputTypeDef,
     ParametersTypeDef,
     ArchiveRuleTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ScheduleOutputTypeDef,
     ScheduleTypeDef,
+    PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
-    CreateLifecyclePolicyRequestRequestTypeDef,
     LifecyclePolicyTypeDef,
+    CreateLifecyclePolicyRequestRequestTypeDef,
+    PolicyDetailsUnionTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierTypeDef:
+def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dlm-2.5.2/types_aiobotocore_dlm.egg-info/SOURCES.txt` & `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


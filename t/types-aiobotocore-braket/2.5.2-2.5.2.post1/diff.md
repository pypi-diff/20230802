# Comparing `tmp/types-aiobotocore-braket-2.5.2.tar.gz` & `tmp/types-aiobotocore-braket-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-braket-2.5.2.tar", last modified: Sat Jul  8 01:43:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-braket-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-braket-2.5.2.tar` & `types-aiobotocore-braket-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.321765 types-aiobotocore-braket-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-08 01:43:18.321765 types-aiobotocore-braket-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:18.321765 types-aiobotocore-braket-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.313764 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-07-08 01:26:25.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-08 01:26:25.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-08 01:26:25.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-08 01:26:25.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-08 01:26:25.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17685 2023-07-08 01:26:26.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-08 01:26:26.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:24.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.321765 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-08 01:43:18.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:43:18.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:18.000000 types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:33:51.000000 types-aiobotocore-braket-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.505643 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-02 14:33:53.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-02 14:33:53.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-08-02 14:33:53.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-braket-2.5.2/LICENSE` & `types-aiobotocore-braket-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/PKG-INFO` & `types-aiobotocore-braket-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-braket
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore braket type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore braket type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-braket"></a>
 
 # types-aiobotocore-braket
 
 [![PyPI - types-aiobotocore-braket](https://img.shields.io/pypi/v/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-braket?color=blue)](https://pypistats.org/packages/types-aiobotocore-braket)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Braket 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
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
@@ -324,57 +323,57 @@
 )
 
 
 def check_value(value: CancellationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_braket.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_braket.type_defs import (
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
-    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
-    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
-    CreateQuantumTaskResponseTypeDef,
     S3DataSourceTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
-    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
     JobEventDetailsTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
-    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
-    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AlgorithmSpecificationTypeDef,
+    CancelJobResponseTypeDef,
+    CancelQuantumTaskResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateQuantumTaskResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetQuantumTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
@@ -383,15 +382,15 @@
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     InputFileConfigTypeDef,
     CreateJobRequestRequestTypeDef,
     GetJobResponseTypeDef,
 )
 
 
-def get_structure() -> ContainerImageTypeDef:
+def get_value() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-braket-2.5.2/README.md` & `types-aiobotocore-braket-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-braket"></a>
 
 # types-aiobotocore-braket
 
 [![PyPI - types-aiobotocore-braket](https://img.shields.io/pypi/v/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-braket?color=blue)](https://pypistats.org/packages/types-aiobotocore-braket)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Braket 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
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
@@ -291,57 +291,57 @@
 )
 
 
 def check_value(value: CancellationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_braket.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_braket.type_defs import (
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
-    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
-    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
-    CreateQuantumTaskResponseTypeDef,
     S3DataSourceTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
-    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
     JobEventDetailsTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
-    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
-    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AlgorithmSpecificationTypeDef,
+    CancelJobResponseTypeDef,
+    CancelQuantumTaskResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateQuantumTaskResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetQuantumTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
@@ -350,15 +350,15 @@
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     InputFileConfigTypeDef,
     CreateJobRequestRequestTypeDef,
     GetJobResponseTypeDef,
 )
 
 
-def get_structure() -> ContainerImageTypeDef:
+def get_value() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-braket-2.5.2/setup.py` & `types-aiobotocore-braket-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-braket",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore braket type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore braket type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_braket": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/"
```

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/__init__.py` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/__init__.pyi` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/__main__.py` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Braket 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Braket 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/client.py` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/client.pyi` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/literals.py` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/literals.pyi` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/paginator.py` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
         """
 
 
@@ -76,15 +76,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
         """
 
 
@@ -94,13 +94,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/paginator.pyi` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
         """
 
 class SearchJobsPaginator(AioPaginator):
@@ -72,15 +72,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
         """
 
 class SearchQuantumTasksPaginator(AioPaginator):
@@ -89,13 +89,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/type_defs.py` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_braket.type_defs import ContainerImageTypeDef
 
-    data: ContainerImageTypeDef = {...}
+    data: ContainerImageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,45 +34,45 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
-    "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
-    "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
-    "CreateQuantumTaskResponseTypeDef",
     "S3DataSourceTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
-    "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
     "JobEventDetailsTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
-    "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AlgorithmSpecificationTypeDef",
+    "CancelJobResponseTypeDef",
+    "CancelQuantumTaskResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateQuantumTaskResponseTypeDef",
+    "GetDeviceResponseTypeDef",
+    "GetQuantumTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
@@ -114,40 +114,33 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancellationStatus": CancellationStatusType,
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelQuantumTaskRequestRequestTypeDef = TypedDict(
     "CancelQuantumTaskRequestRequestTypeDef",
     {
         "clientToken": str,
         "quantumTaskArn": str,
     },
 )
 
-CancelQuantumTaskResponseTypeDef = TypedDict(
-    "CancelQuantumTaskResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigTypeDef = TypedDict(
     "DeviceConfigTypeDef",
     {
         "device": str,
     },
 )
 
@@ -217,22 +210,14 @@
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateQuantumTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuantumTaskRequestRequestTypeDef",
     {
         "action": str,
         "clientToken": str,
         "deviceArn": str,
         "outputS3Bucket": str,
@@ -253,22 +238,14 @@
 
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
 
-CreateQuantumTaskResponseTypeDef = TypedDict(
-    "CreateQuantumTaskResponseTypeDef",
-    {
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
@@ -286,27 +263,14 @@
 GetDeviceRequestRequestTypeDef = TypedDict(
     "GetDeviceRequestRequestTypeDef",
     {
         "deviceArn": str,
     },
 )
 
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "deviceArn": str,
-        "deviceCapabilities": str,
-        "deviceName": str,
-        "deviceStatus": DeviceStatusType,
-        "deviceType": DeviceTypeType,
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
@@ -323,33 +287,14 @@
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
-GetQuantumTaskResponseTypeDef = TypedDict(
-    "GetQuantumTaskResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "deviceArn": str,
-        "deviceParameters": str,
-        "endedAt": datetime,
-        "failureReason": str,
-        "jobArn": str,
-        "outputS3Bucket": str,
-        "outputS3Directory": str,
-        "quantumTaskArn": str,
-        "shots": int,
-        "status": QuantumTaskStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobSummaryTypeDef = TypedDict(
     "_RequiredJobSummaryTypeDef",
     {
         "createdAt": datetime,
         "device": str,
         "jobArn": str,
         "jobName": str,
@@ -374,22 +319,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -420,25 +357,14 @@
 
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
 
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
 SearchDevicesFilterTypeDef = TypedDict(
     "SearchDevicesFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
 )
@@ -482,45 +408,119 @@
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelQuantumTaskResponseTypeDef = TypedDict(
+    "CancelQuantumTaskResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQuantumTaskResponseTypeDef = TypedDict(
+    "CreateQuantumTaskResponseTypeDef",
+    {
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "deviceArn": str,
+        "deviceCapabilities": str,
+        "deviceName": str,
+        "deviceStatus": DeviceStatusType,
+        "deviceType": DeviceTypeType,
+        "providerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQuantumTaskResponseTypeDef = TypedDict(
+    "GetQuantumTaskResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "deviceArn": str,
+        "deviceParameters": str,
+        "endedAt": datetime,
+        "failureReason": str,
+        "jobArn": str,
+        "outputS3Bucket": str,
+        "outputS3Directory": str,
+        "quantumTaskArn": str,
+        "shots": int,
+        "status": QuantumTaskStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
     },
 )
 
 SearchDevicesResponseTypeDef = TypedDict(
     "SearchDevicesResponseTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchJobsResponseTypeDef = TypedDict(
     "SearchJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchQuantumTasksResponseTypeDef = TypedDict(
     "SearchQuantumTasksResponseTypeDef",
     {
         "nextToken": str,
         "quantumTasks": List[QuantumTaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestRequestTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
@@ -547,15 +547,15 @@
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
@@ -591,15 +591,15 @@
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
@@ -636,15 +636,15 @@
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
@@ -722,10 +722,10 @@
         "jobName": str,
         "outputDataConfig": JobOutputDataConfigTypeDef,
         "roleArn": str,
         "startedAt": datetime,
         "status": JobPrimaryStatusType,
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket/type_defs.pyi` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_braket.type_defs import ContainerImageTypeDef
 
-    data: ContainerImageTypeDef = {...}
+    data: ContainerImageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -33,45 +33,45 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
-    "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
-    "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
-    "CreateQuantumTaskResponseTypeDef",
     "S3DataSourceTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
-    "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
     "JobEventDetailsTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
-    "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AlgorithmSpecificationTypeDef",
+    "CancelJobResponseTypeDef",
+    "CancelQuantumTaskResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateQuantumTaskResponseTypeDef",
+    "GetDeviceResponseTypeDef",
+    "GetQuantumTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
@@ -111,40 +111,33 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancellationStatus": CancellationStatusType,
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelQuantumTaskRequestRequestTypeDef = TypedDict(
     "CancelQuantumTaskRequestRequestTypeDef",
     {
         "clientToken": str,
         "quantumTaskArn": str,
     },
 )
 
-CancelQuantumTaskResponseTypeDef = TypedDict(
-    "CancelQuantumTaskResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigTypeDef = TypedDict(
     "DeviceConfigTypeDef",
     {
         "device": str,
     },
 )
 
@@ -208,22 +201,14 @@
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateQuantumTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuantumTaskRequestRequestTypeDef",
     {
         "action": str,
         "clientToken": str,
         "deviceArn": str,
         "outputS3Bucket": str,
@@ -242,22 +227,14 @@
 )
 
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
-CreateQuantumTaskResponseTypeDef = TypedDict(
-    "CreateQuantumTaskResponseTypeDef",
-    {
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
@@ -275,27 +252,14 @@
 GetDeviceRequestRequestTypeDef = TypedDict(
     "GetDeviceRequestRequestTypeDef",
     {
         "deviceArn": str,
     },
 )
 
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "deviceArn": str,
-        "deviceCapabilities": str,
-        "deviceName": str,
-        "deviceStatus": DeviceStatusType,
-        "deviceType": DeviceTypeType,
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
@@ -312,33 +276,14 @@
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
-GetQuantumTaskResponseTypeDef = TypedDict(
-    "GetQuantumTaskResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "deviceArn": str,
-        "deviceParameters": str,
-        "endedAt": datetime,
-        "failureReason": str,
-        "jobArn": str,
-        "outputS3Bucket": str,
-        "outputS3Directory": str,
-        "quantumTaskArn": str,
-        "shots": int,
-        "status": QuantumTaskStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobSummaryTypeDef = TypedDict(
     "_RequiredJobSummaryTypeDef",
     {
         "createdAt": datetime,
         "device": str,
         "jobArn": str,
         "jobName": str,
@@ -361,22 +306,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -405,25 +342,14 @@
 )
 
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
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
 SearchDevicesFilterTypeDef = TypedDict(
     "SearchDevicesFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
 )
@@ -467,45 +393,119 @@
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelQuantumTaskResponseTypeDef = TypedDict(
+    "CancelQuantumTaskResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQuantumTaskResponseTypeDef = TypedDict(
+    "CreateQuantumTaskResponseTypeDef",
+    {
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "deviceArn": str,
+        "deviceCapabilities": str,
+        "deviceName": str,
+        "deviceStatus": DeviceStatusType,
+        "deviceType": DeviceTypeType,
+        "providerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQuantumTaskResponseTypeDef = TypedDict(
+    "GetQuantumTaskResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "deviceArn": str,
+        "deviceParameters": str,
+        "endedAt": datetime,
+        "failureReason": str,
+        "jobArn": str,
+        "outputS3Bucket": str,
+        "outputS3Directory": str,
+        "quantumTaskArn": str,
+        "shots": int,
+        "status": QuantumTaskStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
     },
 )
 
 SearchDevicesResponseTypeDef = TypedDict(
     "SearchDevicesResponseTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchJobsResponseTypeDef = TypedDict(
     "SearchJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchQuantumTasksResponseTypeDef = TypedDict(
     "SearchQuantumTasksResponseTypeDef",
     {
         "nextToken": str,
         "quantumTasks": List[QuantumTaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestRequestTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
@@ -530,15 +530,15 @@
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
     _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef,
@@ -570,15 +570,15 @@
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
     _OptionalSearchJobsRequestSearchJobsPaginateTypeDef,
@@ -611,15 +611,15 @@
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
@@ -691,10 +691,10 @@
         "jobName": str,
         "outputDataConfig": JobOutputDataConfigTypeDef,
         "roleArn": str,
         "startedAt": datetime,
         "status": JobPrimaryStatusType,
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/PKG-INFO` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-braket
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore braket type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore braket type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-braket"></a>
 
 # types-aiobotocore-braket
 
 [![PyPI - types-aiobotocore-braket](https://img.shields.io/pypi/v/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-braket?color=blue)](https://pypistats.org/packages/types-aiobotocore-braket)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Braket 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
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
@@ -324,57 +323,57 @@
 )
 
 
 def check_value(value: CancellationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_braket.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_braket.type_defs import (
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
-    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
-    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
-    CreateQuantumTaskResponseTypeDef,
     S3DataSourceTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
-    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
     JobEventDetailsTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
-    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
-    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AlgorithmSpecificationTypeDef,
+    CancelJobResponseTypeDef,
+    CancelQuantumTaskResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateQuantumTaskResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetQuantumTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
@@ -383,15 +382,15 @@
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     InputFileConfigTypeDef,
     CreateJobRequestRequestTypeDef,
     GetJobResponseTypeDef,
 )
 
 
-def get_structure() -> ContainerImageTypeDef:
+def get_value() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-braket-2.5.2/types_aiobotocore_braket.egg-info/SOURCES.txt` & `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*


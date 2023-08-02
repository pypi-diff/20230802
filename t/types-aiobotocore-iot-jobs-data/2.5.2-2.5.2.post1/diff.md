# Comparing `tmp/types-aiobotocore-iot-jobs-data-2.5.2.tar.gz` & `tmp/types-aiobotocore-iot-jobs-data-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-jobs-data-2.5.2.tar", last modified: Sat Jul  8 01:43:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-jobs-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iot-jobs-data-2.5.2.tar` & `types-aiobotocore-iot-jobs-data-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:45.814286 types-aiobotocore-iot-jobs-data-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-07-08 01:43:45.814286 types-aiobotocore-iot-jobs-data-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:45.814286 types-aiobotocore-iot-jobs-data-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:45.814286 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:34.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:45.814286 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-07-08 01:43:45.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 01:43:45.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:45.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:45.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:45.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:45.000000 types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.121564 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/LICENSE` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/PKG-INFO` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-jobs-data
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot-jobs-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot-jobs-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-jobs-data"></a>
 
 # types-aiobotocore-iot-jobs-data
 
 [![PyPI - types-aiobotocore-iot-jobs-data](https://img.shields.io/pypi/v/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot-jobs-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot-jobs-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-jobs-data)](https://pepy.tech/project/types-aiobotocore-iot-jobs-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTJobsDataPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
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
 [types-aiobotocore-iot-jobs-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/).
 
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
@@ -281,39 +280,39 @@
 )
 
 
 def check_value(value: JobExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot_jobs_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot_jobs_data.type_defs import (
     DescribeJobExecutionRequestRequestTypeDef,
     JobExecutionTypeDef,
+    ResponseMetadataTypeDef,
     GetPendingJobExecutionsRequestRequestTypeDef,
     JobExecutionSummaryTypeDef,
     JobExecutionStateTypeDef,
-    ResponseMetadataTypeDef,
     StartNextPendingJobExecutionRequestRequestTypeDef,
     UpdateJobExecutionRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     StartNextPendingJobExecutionResponseTypeDef,
     GetPendingJobExecutionsResponseTypeDef,
     UpdateJobExecutionResponseTypeDef,
 )
 
 
-def get_structure() -> DescribeJobExecutionRequestRequestTypeDef:
+def get_value() -> DescribeJobExecutionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/README.md` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iot-jobs-data"></a>
 
 # types-aiobotocore-iot-jobs-data
 
 [![PyPI - types-aiobotocore-iot-jobs-data](https://img.shields.io/pypi/v/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot-jobs-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot-jobs-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-jobs-data)](https://pepy.tech/project/types-aiobotocore-iot-jobs-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTJobsDataPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
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
 [types-aiobotocore-iot-jobs-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/).
 
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
@@ -248,39 +248,39 @@
 )
 
 
 def check_value(value: JobExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot_jobs_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot_jobs_data.type_defs import (
     DescribeJobExecutionRequestRequestTypeDef,
     JobExecutionTypeDef,
+    ResponseMetadataTypeDef,
     GetPendingJobExecutionsRequestRequestTypeDef,
     JobExecutionSummaryTypeDef,
     JobExecutionStateTypeDef,
-    ResponseMetadataTypeDef,
     StartNextPendingJobExecutionRequestRequestTypeDef,
     UpdateJobExecutionRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     StartNextPendingJobExecutionResponseTypeDef,
     GetPendingJobExecutionsResponseTypeDef,
     UpdateJobExecutionResponseTypeDef,
 )
 
 
-def get_structure() -> DescribeJobExecutionRequestRequestTypeDef:
+def get_value() -> DescribeJobExecutionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/setup.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-jobs-data",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iot_jobs_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with"
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
-    keywords="aiobotocore iot-jobs-data type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iot-jobs-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot_jobs_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/"
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/__main__.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane\nOther"
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

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/client.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/client.pyi` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/literals.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/literals.pyi` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/type_defs.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestRequestTypeDef
 
-    data: DescribeJobExecutionRequestRequestTypeDef = {...}
+    data: DescribeJobExecutionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping
 
 from .literals import JobExecutionStatusType
 
@@ -21,18 +21,18 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DescribeJobExecutionRequestRequestTypeDef",
     "JobExecutionTypeDef",
+    "ResponseMetadataTypeDef",
     "GetPendingJobExecutionsRequestRequestTypeDef",
     "JobExecutionSummaryTypeDef",
     "JobExecutionStateTypeDef",
-    "ResponseMetadataTypeDef",
     "StartNextPendingJobExecutionRequestRequestTypeDef",
     "UpdateJobExecutionRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "StartNextPendingJobExecutionResponseTypeDef",
     "GetPendingJobExecutionsResponseTypeDef",
     "UpdateJobExecutionResponseTypeDef",
 )
@@ -75,14 +75,25 @@
         "versionNumber": int,
         "executionNumber": int,
         "jobDocument": str,
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
 GetPendingJobExecutionsRequestRequestTypeDef = TypedDict(
     "GetPendingJobExecutionsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
@@ -105,25 +116,14 @@
         "status": JobExecutionStatusType,
         "statusDetails": Dict[str, str],
         "versionNumber": int,
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
 _RequiredStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartNextPendingJobExecutionRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
@@ -172,36 +172,36 @@
     pass
 
 
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartNextPendingJobExecutionResponseTypeDef = TypedDict(
     "StartNextPendingJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPendingJobExecutionsResponseTypeDef = TypedDict(
     "GetPendingJobExecutionsResponseTypeDef",
     {
         "inProgressJobs": List[JobExecutionSummaryTypeDef],
         "queuedJobs": List[JobExecutionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobExecutionResponseTypeDef = TypedDict(
     "UpdateJobExecutionResponseTypeDef",
     {
         "executionState": JobExecutionStateTypeDef,
         "jobDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data/type_defs.pyi` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestRequestTypeDef
 
-    data: DescribeJobExecutionRequestRequestTypeDef = {...}
+    data: DescribeJobExecutionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping
 
 from .literals import JobExecutionStatusType
 
@@ -20,18 +20,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DescribeJobExecutionRequestRequestTypeDef",
     "JobExecutionTypeDef",
+    "ResponseMetadataTypeDef",
     "GetPendingJobExecutionsRequestRequestTypeDef",
     "JobExecutionSummaryTypeDef",
     "JobExecutionStateTypeDef",
-    "ResponseMetadataTypeDef",
     "StartNextPendingJobExecutionRequestRequestTypeDef",
     "UpdateJobExecutionRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "StartNextPendingJobExecutionResponseTypeDef",
     "GetPendingJobExecutionsResponseTypeDef",
     "UpdateJobExecutionResponseTypeDef",
 )
@@ -72,14 +72,25 @@
         "versionNumber": int,
         "executionNumber": int,
         "jobDocument": str,
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
 GetPendingJobExecutionsRequestRequestTypeDef = TypedDict(
     "GetPendingJobExecutionsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
@@ -102,25 +113,14 @@
         "status": JobExecutionStatusType,
         "statusDetails": Dict[str, str],
         "versionNumber": int,
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
 _RequiredStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartNextPendingJobExecutionRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
@@ -165,36 +165,36 @@
 ):
     pass
 
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartNextPendingJobExecutionResponseTypeDef = TypedDict(
     "StartNextPendingJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPendingJobExecutionsResponseTypeDef = TypedDict(
     "GetPendingJobExecutionsResponseTypeDef",
     {
         "inProgressJobs": List[JobExecutionSummaryTypeDef],
         "queuedJobs": List[JobExecutionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobExecutionResponseTypeDef = TypedDict(
     "UpdateJobExecutionResponseTypeDef",
     {
         "executionState": JobExecutionStateTypeDef,
         "jobDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-jobs-data
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot-jobs-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot-jobs-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-jobs-data"></a>
 
 # types-aiobotocore-iot-jobs-data
 
 [![PyPI - types-aiobotocore-iot-jobs-data](https://img.shields.io/pypi/v/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot-jobs-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot-jobs-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-jobs-data)](https://pepy.tech/project/types-aiobotocore-iot-jobs-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTJobsDataPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
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
 [types-aiobotocore-iot-jobs-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/).
 
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
@@ -281,39 +280,39 @@
 )
 
 
 def check_value(value: JobExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot_jobs_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot_jobs_data.type_defs import (
     DescribeJobExecutionRequestRequestTypeDef,
     JobExecutionTypeDef,
+    ResponseMetadataTypeDef,
     GetPendingJobExecutionsRequestRequestTypeDef,
     JobExecutionSummaryTypeDef,
     JobExecutionStateTypeDef,
-    ResponseMetadataTypeDef,
     StartNextPendingJobExecutionRequestRequestTypeDef,
     UpdateJobExecutionRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     StartNextPendingJobExecutionResponseTypeDef,
     GetPendingJobExecutionsResponseTypeDef,
     UpdateJobExecutionResponseTypeDef,
 )
 
 
-def get_structure() -> DescribeJobExecutionRequestRequestTypeDef:
+def get_value() -> DescribeJobExecutionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt` & `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


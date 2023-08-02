# Comparing `tmp/types-aiobotocore-emr-serverless-2.5.2.tar.gz` & `tmp/types-aiobotocore-emr-serverless-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-serverless-2.5.2.tar", last modified: Sat Jul  8 01:43:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-serverless-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
```

## Comparing `types-aiobotocore-emr-serverless-2.5.2.tar` & `types-aiobotocore-emr-serverless-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.510129 types-aiobotocore-emr-serverless-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-07-08 01:43:37.510129 types-aiobotocore-emr-serverless-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:37.510129 types-aiobotocore-emr-serverless-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.506129 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19952 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-08 01:30:40.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:39.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.510129 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-07-08 01:43:37.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:37.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:37.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:37.000000 types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.913588 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/LICENSE` & `types-aiobotocore-emr-serverless-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2/PKG-INFO` & `types-aiobotocore-emr-serverless-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore emr-serverless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-emr-serverless"></a>
 
 # types-aiobotocore-emr-serverless
 
 [![PyPI - types-aiobotocore-emr-serverless](https://img.shields.io/pypi/v/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-emr-serverless?color=blue)](https://pypistats.org/packages/types-aiobotocore-emr-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EMRServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
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
@@ -315,80 +314,89 @@
 )
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_emr_serverless.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationOutputTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    CreateApplicationResponseTypeDef,
+    NetworkConfigurationTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
+    SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    JobDriverUnionTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationSummaryTypeDef:
+def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/README.md` & `types-aiobotocore-emr-serverless-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-emr-serverless"></a>
 
 # types-aiobotocore-emr-serverless
 
 [![PyPI - types-aiobotocore-emr-serverless](https://img.shields.io/pypi/v/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-emr-serverless?color=blue)](https://pypistats.org/packages/types-aiobotocore-emr-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EMRServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
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
@@ -282,80 +282,89 @@
 )
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_emr_serverless.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationOutputTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    CreateApplicationResponseTypeDef,
+    NetworkConfigurationTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
+    SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    JobDriverUnionTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationSummaryTypeDef:
+def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/setup.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-serverless",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with"
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
-    keywords="aiobotocore emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore emr-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_emr_serverless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/"
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/__init__.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/__init__.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/__main__.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMRServerless 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.EMRServerless 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
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

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/client.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 
     session = get_session()
     async with session.create_client("emr-serverless") as client:
         client: EMRServerlessClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
-    JobDriverTypeDef,
+    JobDriverUnionTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     StartJobRunResponseTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -122,15 +122,15 @@
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
@@ -202,16 +202,16 @@
 
     async def list_job_runs(
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#list_job_runs)
@@ -237,16 +237,16 @@
 
     async def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: JobDriverTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        jobDriver: JobDriverUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
@@ -283,15 +283,15 @@
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/client.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 
     session = get_session()
     async with session.create_client("emr-serverless") as client:
         client: EMRServerlessClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
-    JobDriverTypeDef,
+    JobDriverUnionTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     StartJobRunResponseTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -114,15 +114,15 @@
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
@@ -187,16 +187,16 @@
         """
     async def list_job_runs(
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#list_job_runs)
@@ -219,16 +219,16 @@
         """
     async def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: JobDriverTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        jobDriver: JobDriverUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
@@ -261,15 +261,15 @@
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/literals.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/literals.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/paginator.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     with session.create_client("emr-serverless") as client:
         client: EMRServerlessClient
 
         list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
         list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ApplicationStateType, JobRunStateType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListApplicationsPaginator", "ListJobRunsPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -54,15 +54,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -72,16 +72,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/paginator.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     with session.create_client("emr-serverless") as client:
         client: EMRServerlessClient
 
         list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
         list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ApplicationStateType, JobRunStateType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListApplicationsPaginator", "ListJobRunsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -51,15 +51,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(AioPaginator):
@@ -68,16 +68,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/type_defs.py` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_emr_serverless.type_defs import ApplicationSummaryTypeDef
 
-    data: ApplicationSummaryTypeDef = {...}
+    data: ApplicationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
@@ -25,60 +25,69 @@
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
-    "NetworkConfigurationTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "NetworkConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
+    "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
-    "ListJobRunsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListApplicationsResponseTypeDef",
     "WorkerTypeSpecificationTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "InitialCapacityConfigTypeDef",
+    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobRunsRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "JobDriverUnionTypeDef",
+    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
+    "ConfigurationOverridesUnionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
@@ -164,51 +173,75 @@
 
 class MaximumAllowedResourcesTypeDef(
     _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
     {
-        "subnetIds": Sequence[str],
-        "securityGroupIds": Sequence[str],
+        "subnetIds": List[str],
+        "securityGroupIds": List[str],
     },
     total=False,
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+_RequiredConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfigurationOutputTypeDef",
+    {
+        "classification": str,
+    },
+)
+_OptionalConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfigurationOutputTypeDef",
+    {
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
+
+class ConfigurationOutputTypeDef(
+    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
     "_OptionalConfigurationTypeDef",
     {
-        "properties": Dict[str, str],
-        "configurations": List[Dict[str, Any]],
+        "properties": Mapping[str, str],
+        "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
@@ -218,22 +251,21 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
+    total=False,
 )
 
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
@@ -250,22 +282,14 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
@@ -308,24 +332,46 @@
 
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
 
+_RequiredSparkSubmitOutputTypeDef = TypedDict(
+    "_RequiredSparkSubmitOutputTypeDef",
+    {
+        "entryPoint": str,
+    },
+)
+_OptionalSparkSubmitOutputTypeDef = TypedDict(
+    "_OptionalSparkSubmitOutputTypeDef",
+    {
+        "entryPointArguments": List[str],
+        "sparkSubmitParameters": str,
+    },
+    total=False,
+)
+
+
+class SparkSubmitOutputTypeDef(
+    _RequiredSparkSubmitOutputTypeDef, _OptionalSparkSubmitOutputTypeDef
+):
+    pass
+
+
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
     "_OptionalSparkSubmitTypeDef",
     {
-        "entryPointArguments": List[str],
+        "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
 
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
@@ -377,98 +423,42 @@
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestRequestTypeDef(
-    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
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
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
@@ -479,52 +469,21 @@
     {
         "logUri": str,
         "encryptionKeyArn": str,
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -540,39 +499,87 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationTypeDef,
+    },
+    total=False,
+)
+
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -586,32 +593,100 @@
 
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
 
+JobDriverOutputTypeDef = TypedDict(
+    "JobDriverOutputTypeDef",
+    {
+        "sparkSubmit": SparkSubmitOutputTypeDef,
+        "hive": HiveTypeDef,
+    },
+    total=False,
+)
+
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
     },
     total=False,
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
+        "states": Sequence[JobRunStateType],
     },
+    total=False,
 )
 
+
+class ListJobRunsRequestRequestTypeDef(
+    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
+):
+    pass
+
+
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
@@ -637,15 +712,15 @@
         "name": str,
         "stateDetails": str,
         "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
 
@@ -711,36 +786,46 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
+ConfigurationOverridesOutputTypeDef = TypedDict(
+    "ConfigurationOverridesOutputTypeDef",
+    {
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": MonitoringConfigurationTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
-        "applicationConfiguration": List["ConfigurationTypeDef"],
+        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobRunTypeDef = TypedDict(
     "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
@@ -749,37 +834,40 @@
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "jobDriver": JobDriverTypeDef,
+        "jobDriver": JobDriverOutputTypeDef,
     },
 )
 _OptionalJobRunTypeDef = TypedDict(
     "_OptionalJobRunTypeDef",
     {
         "name": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
     total=False,
 )
 
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
 
+ConfigurationOverridesUnionTypeDef = Union[
+    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+]
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
@@ -803,10 +891,10 @@
     pass
 
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless/type_defs.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_emr_serverless.type_defs import ApplicationSummaryTypeDef
 
-    data: ApplicationSummaryTypeDef = {...}
+    data: ApplicationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
@@ -24,60 +24,69 @@
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
-    "NetworkConfigurationTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "NetworkConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
+    "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
-    "ListJobRunsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListApplicationsResponseTypeDef",
     "WorkerTypeSpecificationTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "InitialCapacityConfigTypeDef",
+    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobRunsRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "JobDriverUnionTypeDef",
+    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
+    "ConfigurationOverridesUnionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
@@ -157,51 +166,73 @@
 )
 
 class MaximumAllowedResourcesTypeDef(
     _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
     {
-        "subnetIds": Sequence[str],
-        "securityGroupIds": Sequence[str],
+        "subnetIds": List[str],
+        "securityGroupIds": List[str],
     },
     total=False,
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+_RequiredConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfigurationOutputTypeDef",
+    {
+        "classification": str,
+    },
+)
+_OptionalConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfigurationOutputTypeDef",
+    {
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
     },
+    total=False,
 )
 
+class ConfigurationOutputTypeDef(
+    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
     "_OptionalConfigurationTypeDef",
     {
-        "properties": Dict[str, str],
-        "configurations": List[Dict[str, Any]],
+        "properties": Mapping[str, str],
+        "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
@@ -209,22 +240,21 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
+    total=False,
 )
 
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
@@ -241,22 +271,14 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
@@ -295,24 +317,44 @@
 )
 
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
+_RequiredSparkSubmitOutputTypeDef = TypedDict(
+    "_RequiredSparkSubmitOutputTypeDef",
+    {
+        "entryPoint": str,
+    },
+)
+_OptionalSparkSubmitOutputTypeDef = TypedDict(
+    "_OptionalSparkSubmitOutputTypeDef",
+    {
+        "entryPointArguments": List[str],
+        "sparkSubmitParameters": str,
+    },
+    total=False,
+)
+
+class SparkSubmitOutputTypeDef(
+    _RequiredSparkSubmitOutputTypeDef, _OptionalSparkSubmitOutputTypeDef
+):
+    pass
+
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
     "_OptionalSparkSubmitTypeDef",
     {
-        "entryPointArguments": List[str],
+        "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
     pass
@@ -360,94 +402,42 @@
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-    },
-    total=False,
-)
-
-class ListJobRunsRequestRequestTypeDef(
-    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
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
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
@@ -458,52 +448,21 @@
     {
         "logUri": str,
         "encryptionKeyArn": str,
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -519,39 +478,87 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationTypeDef,
+    },
+    total=False,
+)
+
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -563,31 +570,95 @@
 )
 
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
+JobDriverOutputTypeDef = TypedDict(
+    "JobDriverOutputTypeDef",
+    {
+        "sparkSubmit": SparkSubmitOutputTypeDef,
+        "hive": HiveTypeDef,
+    },
+    total=False,
+)
+
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
     },
     total=False,
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
     },
 )
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
+        "states": Sequence[JobRunStateType],
+    },
+    total=False,
+)
+
+class ListJobRunsRequestRequestTypeDef(
+    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
+):
+    pass
 
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
@@ -614,15 +685,15 @@
         "name": str,
         "stateDetails": str,
         "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
 
@@ -682,36 +753,46 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
+ConfigurationOverridesOutputTypeDef = TypedDict(
+    "ConfigurationOverridesOutputTypeDef",
+    {
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": MonitoringConfigurationTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
-        "applicationConfiguration": List["ConfigurationTypeDef"],
+        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobRunTypeDef = TypedDict(
     "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
@@ -720,35 +801,38 @@
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "jobDriver": JobDriverTypeDef,
+        "jobDriver": JobDriverOutputTypeDef,
     },
 )
 _OptionalJobRunTypeDef = TypedDict(
     "_OptionalJobRunTypeDef",
     {
         "name": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
     total=False,
 )
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
+ConfigurationOverridesUnionTypeDef = Union[
+    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+]
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
@@ -770,10 +854,10 @@
 ):
     pass
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/PKG-INFO` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore emr-serverless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-emr-serverless"></a>
 
 # types-aiobotocore-emr-serverless
 
 [![PyPI - types-aiobotocore-emr-serverless](https://img.shields.io/pypi/v/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-emr-serverless?color=blue)](https://pypistats.org/packages/types-aiobotocore-emr-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EMRServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
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
@@ -315,80 +314,89 @@
 )
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_emr_serverless.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationOutputTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    CreateApplicationResponseTypeDef,
+    NetworkConfigurationTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
+    SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    JobDriverUnionTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationSummaryTypeDef:
+def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*


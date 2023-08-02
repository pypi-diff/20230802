# Comparing `tmp/types-aiobotocore-sagemaker-edge-2.5.2.tar.gz` & `tmp/types-aiobotocore-sagemaker-edge-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-edge-2.5.2.tar", last modified: Sat Jul  8 01:44:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-edge-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-edge-2.5.2.tar` & `types-aiobotocore-sagemaker-edge-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.746840 types-aiobotocore-sagemaker-edge-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-08 01:44:15.742840 types-aiobotocore-sagemaker-edge-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:15.746840 types-aiobotocore-sagemaker-edge-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.742840 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-08 01:40:20.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-08 01:40:22.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-08 01:40:22.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.742840 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.029469 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/LICENSE` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/PKG-INFO` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-edge
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sagemaker-edge type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sagemaker-edge type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sagemaker-edge"></a>
 
 # types-aiobotocore-sagemaker-edge
 
 [![PyPI - types-aiobotocore-sagemaker-edge](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-edge?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-edge)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-edge)](https://pepy.tech/project/types-aiobotocore-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SagemakerEdgeManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [types-aiobotocore-sagemaker-edge docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/).
 
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
@@ -285,41 +284,42 @@
 )
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sagemaker_edge.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
-    EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
+    ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    ResponseMetadataTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
-    ModelTypeDef,
+    EdgeMetricTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
+    ModelTypeDef,
     GetDeploymentsResultTypeDef,
+    SendHeartbeatRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChecksumTypeDef:
+def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/README.md` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sagemaker-edge"></a>
 
 # types-aiobotocore-sagemaker-edge
 
 [![PyPI - types-aiobotocore-sagemaker-edge](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-edge?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-edge)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-edge)](https://pepy.tech/project/types-aiobotocore-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SagemakerEdgeManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [types-aiobotocore-sagemaker-edge docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/).
 
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
@@ -252,41 +252,42 @@
 )
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sagemaker_edge.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
-    EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
+    ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    ResponseMetadataTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
-    ModelTypeDef,
+    EdgeMetricTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
+    ModelTypeDef,
     GetDeploymentsResultTypeDef,
+    SendHeartbeatRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChecksumTypeDef:
+def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/setup.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-edge",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sagemaker_edge"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with"
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
-    keywords="aiobotocore sagemaker-edge type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sagemaker-edge type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sagemaker_edge": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/"
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/__init__.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/__init__.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/__main__.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager\nOther"
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

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/client.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/client.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/literals.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/literals.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/type_defs.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sagemaker_edge.type_defs import ChecksumTypeDef
 
-    data: ChecksumTypeDef = {...}
+    data: ChecksumTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import DeploymentStatusType, FailureHandlingPolicyType, ModelStateType
@@ -26,26 +26,27 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChecksumTypeDef",
     "DeploymentModelTypeDef",
-    "EdgeMetricTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
+    "ResponseMetadataTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDeviceRegistrationRequestRequestTypeDef",
-    "GetDeviceRegistrationResultTypeDef",
-    "ResponseMetadataTypeDef",
     "DefinitionTypeDef",
     "DeploymentResultTypeDef",
-    "ModelTypeDef",
+    "EdgeMetricTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDeviceRegistrationResultTypeDef",
     "EdgeDeploymentTypeDef",
-    "SendHeartbeatRequestRequestTypeDef",
+    "ModelTypeDef",
     "GetDeploymentsResultTypeDef",
+    "SendHeartbeatRequestRequestTypeDef",
 )
 
 ChecksumTypeDef = TypedDict(
     "ChecksumTypeDef",
     {
         "Type": Literal["SHA1"],
         "Sum": str,
@@ -64,29 +65,23 @@
         "Status": DeploymentStatusType,
         "StatusReason": str,
         "RollbackFailureReason": str,
     },
     total=False,
 )
 
-EdgeMetricTypeDef = TypedDict(
-    "EdgeMetricTypeDef",
-    {
-        "Dimension": str,
-        "MetricName": str,
-        "Value": float,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TimestampTypeDef = Union[datetime, str]
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetDeploymentsRequestRequestTypeDef = TypedDict(
     "GetDeploymentsRequestRequestTypeDef",
     {
         "DeviceName": str,
@@ -98,34 +93,14 @@
     "GetDeviceRegistrationRequestRequestTypeDef",
     {
         "DeviceName": str,
         "DeviceFleetName": str,
     },
 )
 
-GetDeviceRegistrationResultTypeDef = TypedDict(
-    "GetDeviceRegistrationResultTypeDef",
-    {
-        "DeviceRegistration": str,
-        "CacheTTL": str,
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
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "ModelHandle": str,
         "S3Url": str,
         "Checksum": ChecksumTypeDef,
         "State": ModelStateType,
@@ -135,44 +110,79 @@
 
 DeploymentResultTypeDef = TypedDict(
     "DeploymentResultTypeDef",
     {
         "DeploymentName": str,
         "DeploymentStatus": str,
         "DeploymentStatusMessage": str,
-        "DeploymentStartTime": Union[datetime, str],
-        "DeploymentEndTime": Union[datetime, str],
+        "DeploymentStartTime": TimestampTypeDef,
+        "DeploymentEndTime": TimestampTypeDef,
         "DeploymentModels": Sequence[DeploymentModelTypeDef],
     },
     total=False,
 )
 
-ModelTypeDef = TypedDict(
-    "ModelTypeDef",
+EdgeMetricTypeDef = TypedDict(
+    "EdgeMetricTypeDef",
     {
-        "ModelName": str,
-        "ModelVersion": str,
-        "LatestSampleTime": Union[datetime, str],
-        "LatestInference": Union[datetime, str],
-        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+        "Dimension": str,
+        "MetricName": str,
+        "Value": float,
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceRegistrationResultTypeDef = TypedDict(
+    "GetDeviceRegistrationResultTypeDef",
+    {
+        "DeviceRegistration": str,
+        "CacheTTL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeDeploymentTypeDef = TypedDict(
     "EdgeDeploymentTypeDef",
     {
         "DeploymentName": str,
         "Type": Literal["Model"],
         "FailureHandlingPolicy": FailureHandlingPolicyType,
         "Definitions": List[DefinitionTypeDef],
     },
     total=False,
 )
 
+ModelTypeDef = TypedDict(
+    "ModelTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": str,
+        "LatestSampleTime": TimestampTypeDef,
+        "LatestInference": TimestampTypeDef,
+        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+    },
+    total=False,
+)
+
+GetDeploymentsResultTypeDef = TypedDict(
+    "GetDeploymentsResultTypeDef",
+    {
+        "Deployments": List[EdgeDeploymentTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredSendHeartbeatRequestRequestTypeDef = TypedDict(
     "_RequiredSendHeartbeatRequestRequestTypeDef",
     {
         "AgentVersion": str,
         "DeviceName": str,
         "DeviceFleetName": str,
     },
@@ -188,16 +198,7 @@
 )
 
 
 class SendHeartbeatRequestRequestTypeDef(
     _RequiredSendHeartbeatRequestRequestTypeDef, _OptionalSendHeartbeatRequestRequestTypeDef
 ):
     pass
-
-
-GetDeploymentsResultTypeDef = TypedDict(
-    "GetDeploymentsResultTypeDef",
-    {
-        "Deployments": List[EdgeDeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge/type_defs.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sagemaker_edge.type_defs import ChecksumTypeDef
 
-    data: ChecksumTypeDef = {...}
+    data: ChecksumTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import DeploymentStatusType, FailureHandlingPolicyType, ModelStateType
@@ -25,26 +25,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChecksumTypeDef",
     "DeploymentModelTypeDef",
-    "EdgeMetricTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
+    "ResponseMetadataTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDeviceRegistrationRequestRequestTypeDef",
-    "GetDeviceRegistrationResultTypeDef",
-    "ResponseMetadataTypeDef",
     "DefinitionTypeDef",
     "DeploymentResultTypeDef",
-    "ModelTypeDef",
+    "EdgeMetricTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDeviceRegistrationResultTypeDef",
     "EdgeDeploymentTypeDef",
-    "SendHeartbeatRequestRequestTypeDef",
+    "ModelTypeDef",
     "GetDeploymentsResultTypeDef",
+    "SendHeartbeatRequestRequestTypeDef",
 )
 
 ChecksumTypeDef = TypedDict(
     "ChecksumTypeDef",
     {
         "Type": Literal["SHA1"],
         "Sum": str,
@@ -63,29 +64,23 @@
         "Status": DeploymentStatusType,
         "StatusReason": str,
         "RollbackFailureReason": str,
     },
     total=False,
 )
 
-EdgeMetricTypeDef = TypedDict(
-    "EdgeMetricTypeDef",
-    {
-        "Dimension": str,
-        "MetricName": str,
-        "Value": float,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TimestampTypeDef = Union[datetime, str]
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetDeploymentsRequestRequestTypeDef = TypedDict(
     "GetDeploymentsRequestRequestTypeDef",
     {
         "DeviceName": str,
@@ -97,34 +92,14 @@
     "GetDeviceRegistrationRequestRequestTypeDef",
     {
         "DeviceName": str,
         "DeviceFleetName": str,
     },
 )
 
-GetDeviceRegistrationResultTypeDef = TypedDict(
-    "GetDeviceRegistrationResultTypeDef",
-    {
-        "DeviceRegistration": str,
-        "CacheTTL": str,
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
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "ModelHandle": str,
         "S3Url": str,
         "Checksum": ChecksumTypeDef,
         "State": ModelStateType,
@@ -134,44 +109,79 @@
 
 DeploymentResultTypeDef = TypedDict(
     "DeploymentResultTypeDef",
     {
         "DeploymentName": str,
         "DeploymentStatus": str,
         "DeploymentStatusMessage": str,
-        "DeploymentStartTime": Union[datetime, str],
-        "DeploymentEndTime": Union[datetime, str],
+        "DeploymentStartTime": TimestampTypeDef,
+        "DeploymentEndTime": TimestampTypeDef,
         "DeploymentModels": Sequence[DeploymentModelTypeDef],
     },
     total=False,
 )
 
-ModelTypeDef = TypedDict(
-    "ModelTypeDef",
+EdgeMetricTypeDef = TypedDict(
+    "EdgeMetricTypeDef",
     {
-        "ModelName": str,
-        "ModelVersion": str,
-        "LatestSampleTime": Union[datetime, str],
-        "LatestInference": Union[datetime, str],
-        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+        "Dimension": str,
+        "MetricName": str,
+        "Value": float,
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceRegistrationResultTypeDef = TypedDict(
+    "GetDeviceRegistrationResultTypeDef",
+    {
+        "DeviceRegistration": str,
+        "CacheTTL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeDeploymentTypeDef = TypedDict(
     "EdgeDeploymentTypeDef",
     {
         "DeploymentName": str,
         "Type": Literal["Model"],
         "FailureHandlingPolicy": FailureHandlingPolicyType,
         "Definitions": List[DefinitionTypeDef],
     },
     total=False,
 )
 
+ModelTypeDef = TypedDict(
+    "ModelTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": str,
+        "LatestSampleTime": TimestampTypeDef,
+        "LatestInference": TimestampTypeDef,
+        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+    },
+    total=False,
+)
+
+GetDeploymentsResultTypeDef = TypedDict(
+    "GetDeploymentsResultTypeDef",
+    {
+        "Deployments": List[EdgeDeploymentTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredSendHeartbeatRequestRequestTypeDef = TypedDict(
     "_RequiredSendHeartbeatRequestRequestTypeDef",
     {
         "AgentVersion": str,
         "DeviceName": str,
         "DeviceFleetName": str,
     },
@@ -186,15 +196,7 @@
     total=False,
 )
 
 class SendHeartbeatRequestRequestTypeDef(
     _RequiredSendHeartbeatRequestRequestTypeDef, _OptionalSendHeartbeatRequestRequestTypeDef
 ):
     pass
-
-GetDeploymentsResultTypeDef = TypedDict(
-    "GetDeploymentsResultTypeDef",
-    {
-        "Deployments": List[EdgeDeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-edge
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sagemaker-edge type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sagemaker-edge type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sagemaker-edge"></a>
 
 # types-aiobotocore-sagemaker-edge
 
 [![PyPI - types-aiobotocore-sagemaker-edge](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-edge?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-edge)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-edge)](https://pepy.tech/project/types-aiobotocore-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SagemakerEdgeManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [types-aiobotocore-sagemaker-edge docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/).
 
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
@@ -285,41 +284,42 @@
 )
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sagemaker_edge.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
-    EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
+    ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    ResponseMetadataTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
-    ModelTypeDef,
+    EdgeMetricTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
+    ModelTypeDef,
     GetDeploymentsResultTypeDef,
+    SendHeartbeatRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChecksumTypeDef:
+def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*


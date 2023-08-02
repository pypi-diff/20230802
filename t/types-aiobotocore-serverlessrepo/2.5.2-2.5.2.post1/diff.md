# Comparing `tmp/types-aiobotocore-serverlessrepo-2.5.2.tar.gz` & `tmp/types-aiobotocore-serverlessrepo-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-serverlessrepo-2.5.2.tar", last modified: Sat Jul  8 01:44:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-serverlessrepo-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
```

## Comparing `types-aiobotocore-serverlessrepo-2.5.2.tar` & `types-aiobotocore-serverlessrepo-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.338886 types-aiobotocore-serverlessrepo-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-08 01:44:18.338886 types-aiobotocore-serverlessrepo-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:18.338886 types-aiobotocore-serverlessrepo-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.334885 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-08 01:40:50.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:49.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.338886 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-08 01:44:18.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:18.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:18.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:18.000000 types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.685461 types-aiobotocore-serverlessrepo-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-08-02 14:52:59.677461 types-aiobotocore-serverlessrepo-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.685461 types-aiobotocore-serverlessrepo-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.677461 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-02 14:49:30.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-08-02 14:49:30.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.677461 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/LICENSE` & `types-aiobotocore-serverlessrepo-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore serverlessrepo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore serverlessrepo type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-serverlessrepo"></a>
 
 # types-aiobotocore-serverlessrepo
 
 [![PyPI - types-aiobotocore-serverlessrepo](https://img.shields.io/pypi/v/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-serverlessrepo?color=blue)](https://pypistats.org/packages/types-aiobotocore-serverlessrepo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServerlessApplicationRepository 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
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
@@ -321,69 +320,71 @@
 )
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_serverlessrepo.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    PutApplicationPolicyResponseTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    PutApplicationPolicyResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ApplicationDependencySummaryTypeDef:
+def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/README.md` & `types-aiobotocore-serverlessrepo-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-serverlessrepo"></a>
 
 # types-aiobotocore-serverlessrepo
 
 [![PyPI - types-aiobotocore-serverlessrepo](https://img.shields.io/pypi/v/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-serverlessrepo?color=blue)](https://pypistats.org/packages/types-aiobotocore-serverlessrepo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServerlessApplicationRepository 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
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
@@ -288,69 +288,71 @@
 )
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_serverlessrepo.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    PutApplicationPolicyResponseTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    PutApplicationPolicyResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ApplicationDependencySummaryTypeDef:
+def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/setup.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-serverlessrepo",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated"
-        " with mypy-boto3-builder 7.14.5"
+        " with mypy-boto3-builder 7.17.1"
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
-    keywords="aiobotocore serverlessrepo type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore serverlessrepo type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_serverlessrepo": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/"
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/__init__.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/__init__.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/__main__.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/client.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
-    ApplicationPolicyStatementTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetApplicationResponseTypeDef,
@@ -267,15 +267,15 @@
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#list_applications)
         """
 
     async def put_application_policy(
-        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementTypeDef]
+        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementUnionTypeDef]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/client.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
-    ApplicationPolicyStatementTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetApplicationResponseTypeDef,
@@ -248,15 +248,15 @@
         """
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#list_applications)
         """
     async def put_application_policy(
-        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementTypeDef]
+        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementUnionTypeDef]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/literals.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/literals.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/paginator.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,65 +38,60 @@
 
 __all__ = (
     "ListApplicationDependenciesPaginator",
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListApplicationDependenciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationdependenciespaginator)
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
-
 class ListApplicationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationversionspaginator)
         """
 
-
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationspaginator)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/paginator.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,60 +38,65 @@
 
 __all__ = (
     "ListApplicationDependenciesPaginator",
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListApplicationDependenciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationdependenciespaginator)
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
+
 class ListApplicationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationversionspaginator)
         """
 
+
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationspaginator)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/type_defs.py` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,104 +4,125 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
-    data: ApplicationDependencySummaryTypeDef = {...}
+    data: ApplicationDependencySummaryTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
+    "ApplicationPolicyStatementOutputTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateRequestRequestTypeDef",
-    "CreateCloudFormationTemplateResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetCloudFormationTemplateRequestRequestTypeDef",
-    "GetCloudFormationTemplateResponseTypeDef",
-    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationDependenciesRequestRequestTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "ListApplicationDependenciesResponseTypeDef",
+    "ApplicationPolicyStatementUnionTypeDef",
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    "CreateCloudFormationTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyResponseTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
-    "PutApplicationPolicyResponseTypeDef",
+    "GetCloudFormationTemplateResponseTypeDef",
+    "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
+    "PutApplicationPolicyResponseTypeDef",
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
+    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
 
 ApplicationDependencySummaryTypeDef = TypedDict(
     "ApplicationDependencySummaryTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
 
-_RequiredApplicationPolicyStatementTypeDef = TypedDict(
-    "_RequiredApplicationPolicyStatementTypeDef",
+_RequiredApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementOutputTypeDef",
     {
         "Actions": List[str],
         "Principals": List[str],
     },
 )
-_OptionalApplicationPolicyStatementTypeDef = TypedDict(
-    "_OptionalApplicationPolicyStatementTypeDef",
+_OptionalApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_OptionalApplicationPolicyStatementOutputTypeDef",
     {
         "PrincipalOrgIDs": List[str],
         "StatementId": str,
     },
     total=False,
 )
 
+class ApplicationPolicyStatementOutputTypeDef(
+    _RequiredApplicationPolicyStatementOutputTypeDef,
+    _OptionalApplicationPolicyStatementOutputTypeDef,
+):
+    pass
+
+_RequiredApplicationPolicyStatementTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementTypeDef",
+    {
+        "Actions": Sequence[str],
+        "Principals": Sequence[str],
+    },
+)
+_OptionalApplicationPolicyStatementTypeDef = TypedDict(
+    "_OptionalApplicationPolicyStatementTypeDef",
+    {
+        "PrincipalOrgIDs": Sequence[str],
+        "StatementId": str,
+    },
+    total=False,
+)
 
 class ApplicationPolicyStatementTypeDef(
     _RequiredApplicationPolicyStatementTypeDef, _OptionalApplicationPolicyStatementTypeDef
 ):
     pass
 
-
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "Description": str,
         "Name": str,
@@ -114,21 +135,19 @@
         "HomePageUrl": str,
         "Labels": List[str],
         "SpdxLicenseId": str,
     },
     total=False,
 )
 
-
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Author": str,
         "Description": str,
         "Name": str,
     },
@@ -148,20 +167,29 @@
         "SpdxLicenseId": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
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
 
 _RequiredCreateApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
@@ -173,22 +201,20 @@
         "SourceCodeUrl": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
-
 class CreateApplicationVersionRequestRequestTypeDef(
     _RequiredCreateApplicationVersionRequestRequestTypeDef,
     _OptionalCreateApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredParameterDefinitionTypeDef = TypedDict(
     "_RequiredParameterDefinitionTypeDef",
     {
         "Name": str,
         "ReferencedByResources": List[str],
     },
 )
@@ -206,21 +232,19 @@
         "MinValue": int,
         "NoEcho": bool,
         "Type": str,
     },
     total=False,
 )
 
-
 class ParameterDefinitionTypeDef(
     _RequiredParameterDefinitionTypeDef, _OptionalParameterDefinitionTypeDef
 ):
     pass
 
-
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -229,75 +253,41 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "ChangeSetId": str,
-        "SemanticVersion": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
-
 class CreateCloudFormationTemplateRequestRequestTypeDef(
     _RequiredCreateCloudFormationTemplateRequestRequestTypeDef,
     _OptionalCreateCloudFormationTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-CreateCloudFormationTemplateResponseTypeDef = TypedDict(
-    "CreateCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationPolicyRequestRequestTypeDef = TypedDict(
     "GetApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -311,66 +301,37 @@
     "_OptionalGetApplicationRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
-
 class GetApplicationRequestRequestTypeDef(
     _RequiredGetApplicationRequestRequestTypeDef, _OptionalGetApplicationRequestRequestTypeDef
 ):
     pass
 
-
 GetCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "GetCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "TemplateId": str,
     },
 )
 
-GetCloudFormationTemplateResponseTypeDef = TypedDict(
-    "GetCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SemanticVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
-    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationDependenciesRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationDependenciesRequestRequestTypeDef = TypedDict(
@@ -379,44 +340,20 @@
         "MaxItems": int,
         "NextToken": str,
         "SemanticVersion": str,
     },
     total=False,
 )
 
-
 class ListApplicationDependenciesRequestRequestTypeDef(
     _RequiredListApplicationDependenciesRequestRequestTypeDef,
     _OptionalListApplicationDependenciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -424,22 +361,20 @@
     {
         "MaxItems": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredVersionSummaryTypeDef = TypedDict(
     "_RequiredVersionSummaryTypeDef",
     {
         "ApplicationId": str,
         "CreationTime": str,
         "SemanticVersion": str,
     },
@@ -448,57 +383,26 @@
     "_OptionalVersionSummaryTypeDef",
     {
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
-
 class VersionSummaryTypeDef(_RequiredVersionSummaryTypeDef, _OptionalVersionSummaryTypeDef):
     pass
 
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "NextToken": str,
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
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -526,60 +430,99 @@
         "Labels": Sequence[str],
         "ReadmeBody": str,
         "ReadmeUrl": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+ApplicationPolicyStatementUnionTypeDef = Union[
+    ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef
+]
+CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "ChangeSetId": str,
+        "SemanticVersion": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListApplicationDependenciesResponseTypeDef = TypedDict(
-    "ListApplicationDependenciesResponseTypeDef",
+CreateCloudFormationTemplateResponseTypeDef = TypedDict(
+    "CreateCloudFormationTemplateResponseTypeDef",
     {
-        "Dependencies": List[ApplicationDependencySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
+GetCloudFormationTemplateResponseTypeDef = TypedDict(
+    "GetCloudFormationTemplateResponseTypeDef",
     {
         "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyResponseTypeDef = TypedDict(
-    "PutApplicationPolicyResponseTypeDef",
+ListApplicationDependenciesResponseTypeDef = TypedDict(
+    "ListApplicationDependenciesResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Dependencies": List[ApplicationDependencySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutApplicationPolicyResponseTypeDef = TypedDict(
+    "PutApplicationPolicyResponseTypeDef",
+    {
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
         "ApplicationId": str,
@@ -587,15 +530,15 @@
         "ParameterDefinitions": List[ParameterDefinitionTypeDef],
         "RequiredCapabilities": List[CapabilityType],
         "ResourcesSupported": bool,
         "SemanticVersion": str,
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
         "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVersionTypeDef = TypedDict(
     "_RequiredVersionTypeDef",
     {
         "ApplicationId": str,
@@ -612,37 +555,92 @@
     {
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
-
 class VersionTypeDef(_RequiredVersionTypeDef, _OptionalVersionTypeDef):
     pass
 
+_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "SemanticVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
+    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "MonitoringTimeInMinutes": int,
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
     },
     total=False,
 )
 
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementUnionTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "CreationTime": str,
         "Description": str,
@@ -651,15 +649,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -671,15 +669,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -691,15 +689,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationChangeSetRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -720,13 +718,12 @@
         "SemanticVersion": str,
         "Tags": Sequence[TagTypeDef],
         "TemplateId": str,
     },
     total=False,
 )
 
-
 class CreateCloudFormationChangeSetRequestRequestTypeDef(
     _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef,
     _OptionalCreateCloudFormationChangeSetRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo/type_defs.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,101 +4,130 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
-    data: ApplicationDependencySummaryTypeDef = {...}
+    data: ApplicationDependencySummaryTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
+    "ApplicationPolicyStatementOutputTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateRequestRequestTypeDef",
-    "CreateCloudFormationTemplateResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetCloudFormationTemplateRequestRequestTypeDef",
-    "GetCloudFormationTemplateResponseTypeDef",
-    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationDependenciesRequestRequestTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "ListApplicationDependenciesResponseTypeDef",
+    "ApplicationPolicyStatementUnionTypeDef",
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    "CreateCloudFormationTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyResponseTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
-    "PutApplicationPolicyResponseTypeDef",
+    "GetCloudFormationTemplateResponseTypeDef",
+    "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
+    "PutApplicationPolicyResponseTypeDef",
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
+    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
 
 ApplicationDependencySummaryTypeDef = TypedDict(
     "ApplicationDependencySummaryTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
 
-_RequiredApplicationPolicyStatementTypeDef = TypedDict(
-    "_RequiredApplicationPolicyStatementTypeDef",
+_RequiredApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementOutputTypeDef",
     {
         "Actions": List[str],
         "Principals": List[str],
     },
 )
+_OptionalApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_OptionalApplicationPolicyStatementOutputTypeDef",
+    {
+        "PrincipalOrgIDs": List[str],
+        "StatementId": str,
+    },
+    total=False,
+)
+
+
+class ApplicationPolicyStatementOutputTypeDef(
+    _RequiredApplicationPolicyStatementOutputTypeDef,
+    _OptionalApplicationPolicyStatementOutputTypeDef,
+):
+    pass
+
+
+_RequiredApplicationPolicyStatementTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementTypeDef",
+    {
+        "Actions": Sequence[str],
+        "Principals": Sequence[str],
+    },
+)
 _OptionalApplicationPolicyStatementTypeDef = TypedDict(
     "_OptionalApplicationPolicyStatementTypeDef",
     {
-        "PrincipalOrgIDs": List[str],
+        "PrincipalOrgIDs": Sequence[str],
         "StatementId": str,
     },
     total=False,
 )
 
+
 class ApplicationPolicyStatementTypeDef(
     _RequiredApplicationPolicyStatementTypeDef, _OptionalApplicationPolicyStatementTypeDef
 ):
     pass
 
+
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "Description": str,
         "Name": str,
@@ -111,19 +140,21 @@
         "HomePageUrl": str,
         "Labels": List[str],
         "SpdxLicenseId": str,
     },
     total=False,
 )
 
+
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Author": str,
         "Description": str,
         "Name": str,
     },
@@ -143,19 +174,32 @@
         "SpdxLicenseId": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
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
 _RequiredCreateApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
@@ -166,20 +210,22 @@
         "SourceCodeUrl": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
+
 class CreateApplicationVersionRequestRequestTypeDef(
     _RequiredCreateApplicationVersionRequestRequestTypeDef,
     _OptionalCreateApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredParameterDefinitionTypeDef = TypedDict(
     "_RequiredParameterDefinitionTypeDef",
     {
         "Name": str,
         "ReferencedByResources": List[str],
     },
 )
@@ -197,19 +243,21 @@
         "MinValue": int,
         "NoEcho": bool,
         "Type": str,
     },
     total=False,
 )
 
+
 class ParameterDefinitionTypeDef(
     _RequiredParameterDefinitionTypeDef, _OptionalParameterDefinitionTypeDef
 ):
     pass
 
+
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -218,73 +266,43 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "ChangeSetId": str,
-        "SemanticVersion": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
+
 class CreateCloudFormationTemplateRequestRequestTypeDef(
     _RequiredCreateCloudFormationTemplateRequestRequestTypeDef,
     _OptionalCreateCloudFormationTemplateRequestRequestTypeDef,
 ):
     pass
 
-CreateCloudFormationTemplateResponseTypeDef = TypedDict(
-    "CreateCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationPolicyRequestRequestTypeDef = TypedDict(
     "GetApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -298,62 +316,39 @@
     "_OptionalGetApplicationRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
+
 class GetApplicationRequestRequestTypeDef(
     _RequiredGetApplicationRequestRequestTypeDef, _OptionalGetApplicationRequestRequestTypeDef
 ):
     pass
 
+
 GetCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "GetCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "TemplateId": str,
     },
 )
 
-GetCloudFormationTemplateResponseTypeDef = TypedDict(
-    "GetCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SemanticVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
-    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationDependenciesRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationDependenciesRequestRequestTypeDef = TypedDict(
@@ -362,39 +357,21 @@
         "MaxItems": int,
         "NextToken": str,
         "SemanticVersion": str,
     },
     total=False,
 )
 
+
 class ListApplicationDependenciesRequestRequestTypeDef(
     _RequiredListApplicationDependenciesRequestRequestTypeDef,
     _OptionalListApplicationDependenciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
@@ -403,20 +380,22 @@
     {
         "MaxItems": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredVersionSummaryTypeDef = TypedDict(
     "_RequiredVersionSummaryTypeDef",
     {
         "ApplicationId": str,
         "CreationTime": str,
         "SemanticVersion": str,
     },
@@ -425,55 +404,28 @@
     "_OptionalVersionSummaryTypeDef",
     {
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
+
 class VersionSummaryTypeDef(_RequiredVersionSummaryTypeDef, _OptionalVersionSummaryTypeDef):
     pass
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "NextToken": str,
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
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -501,58 +453,101 @@
         "Labels": Sequence[str],
         "ReadmeBody": str,
         "ReadmeUrl": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-ListApplicationDependenciesResponseTypeDef = TypedDict(
-    "ListApplicationDependenciesResponseTypeDef",
+
+ApplicationPolicyStatementUnionTypeDef = Union[
+    ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef
+]
+CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
+    "CreateCloudFormationChangeSetResponseTypeDef",
     {
-        "Dependencies": List[ApplicationDependencySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationId": str,
+        "ChangeSetId": str,
+        "SemanticVersion": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCloudFormationTemplateResponseTypeDef = TypedDict(
+    "CreateCloudFormationTemplateResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
+GetCloudFormationTemplateResponseTypeDef = TypedDict(
+    "GetCloudFormationTemplateResponseTypeDef",
     {
         "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyResponseTypeDef = TypedDict(
-    "PutApplicationPolicyResponseTypeDef",
+ListApplicationDependenciesResponseTypeDef = TypedDict(
+    "ListApplicationDependenciesResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Dependencies": List[ApplicationDependencySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutApplicationPolicyResponseTypeDef = TypedDict(
+    "PutApplicationPolicyResponseTypeDef",
+    {
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
         "ApplicationId": str,
@@ -560,15 +555,15 @@
         "ParameterDefinitions": List[ParameterDefinitionTypeDef],
         "RequiredCapabilities": List[CapabilityType],
         "ResourcesSupported": bool,
         "SemanticVersion": str,
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
         "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVersionTypeDef = TypedDict(
     "_RequiredVersionTypeDef",
     {
         "ApplicationId": str,
@@ -585,35 +580,98 @@
     {
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
+
 class VersionTypeDef(_RequiredVersionTypeDef, _OptionalVersionTypeDef):
     pass
 
+
+_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "SemanticVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
+    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "MonitoringTimeInMinutes": int,
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
     },
     total=False,
 )
 
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementUnionTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "CreationTime": str,
         "Description": str,
@@ -622,15 +680,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -642,15 +700,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -662,15 +720,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationChangeSetRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -691,12 +749,13 @@
         "SemanticVersion": str,
         "Tags": Sequence[TagTypeDef],
         "TemplateId": str,
     },
     total=False,
 )
 
+
 class CreateCloudFormationChangeSetRequestRequestTypeDef(
     _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef,
     _OptionalCreateCloudFormationChangeSetRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore serverlessrepo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore serverlessrepo type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-serverlessrepo"></a>
 
 # types-aiobotocore-serverlessrepo
 
 [![PyPI - types-aiobotocore-serverlessrepo](https://img.shields.io/pypi/v/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-serverlessrepo?color=blue)](https://pypistats.org/packages/types-aiobotocore-serverlessrepo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServerlessApplicationRepository 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
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
@@ -321,69 +320,71 @@
 )
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_serverlessrepo.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    PutApplicationPolicyResponseTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    PutApplicationPolicyResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ApplicationDependencySummaryTypeDef:
+def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt` & `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


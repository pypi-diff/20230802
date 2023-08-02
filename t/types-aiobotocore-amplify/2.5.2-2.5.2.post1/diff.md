# Comparing `tmp/types-aiobotocore-amplify-2.5.2.tar.gz` & `tmp/types-aiobotocore-amplify-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplify-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplify-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
```

## Comparing `types-aiobotocore-amplify-2.5.2.tar` & `types-aiobotocore-amplify-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.833605 types-aiobotocore-amplify-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-08 01:43:09.833605 types-aiobotocore-amplify-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.833605 types-aiobotocore-amplify-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.833605 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35286 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-07-08 01:25:24.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:23.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.833605 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-08 01:43:09.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:09.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:09.000000 types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-amplify-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-08-02 14:51:47.833667 types-aiobotocore-amplify-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.841667 types-aiobotocore-amplify-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29862 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36050 2023-08-02 14:32:51.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35991 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplify-2.5.2/LICENSE` & `types-aiobotocore-amplify-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/PKG-INFO` & `types-aiobotocore-amplify-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplify
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Amplify 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Amplify 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore amplify type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore amplify type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amplify"></a>
 
 # types-aiobotocore-amplify
 
 [![PyPI - types-aiobotocore-amplify](https://img.shields.io/pypi/v/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplify?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplify)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplify)](https://pepy.tech/project/types-aiobotocore-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Amplify 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [types-aiobotocore-amplify docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/).
 
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
@@ -323,27 +322,28 @@
 )
 
 
 def check_value(value: DomainStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplify.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplify.type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigOutputTypeDef,
     CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
+    AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
@@ -352,15 +352,15 @@
     DeleteAppRequestRequestTypeDef,
     DeleteBackendEnvironmentRequestRequestTypeDef,
     DeleteBranchRequestRequestTypeDef,
     DeleteDomainAssociationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     JobSummaryTypeDef,
     DeleteWebhookRequestRequestTypeDef,
-    GenerateAccessLogsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetAppRequestRequestTypeDef,
     GetArtifactUrlRequestRequestTypeDef,
     GetBackendEnvironmentRequestRequestTypeDef,
     GetBranchRequestRequestTypeDef,
     GetDomainAssociationRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetWebhookRequestRequestTypeDef,
@@ -371,23 +371,23 @@
     ListBackendEnvironmentsRequestRequestTypeDef,
     ListBranchesRequestRequestTypeDef,
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
+    AppTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
-    AppTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
     GenerateAccessLogsResultTypeDef,
     GetArtifactUrlResultTypeDef,
@@ -407,14 +407,16 @@
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
     ListJobsResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
+    GenerateAccessLogsRequestRequestTypeDef,
+    StartJobRequestRequestTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
@@ -427,15 +429,15 @@
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplify-2.5.2/README.md` & `types-aiobotocore-amplify-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-amplify"></a>
 
 # types-aiobotocore-amplify
 
 [![PyPI - types-aiobotocore-amplify](https://img.shields.io/pypi/v/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplify?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplify)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplify)](https://pepy.tech/project/types-aiobotocore-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Amplify 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [types-aiobotocore-amplify docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/).
 
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
@@ -290,27 +290,28 @@
 )
 
 
 def check_value(value: DomainStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplify.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplify.type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigOutputTypeDef,
     CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
+    AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
@@ -319,15 +320,15 @@
     DeleteAppRequestRequestTypeDef,
     DeleteBackendEnvironmentRequestRequestTypeDef,
     DeleteBranchRequestRequestTypeDef,
     DeleteDomainAssociationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     JobSummaryTypeDef,
     DeleteWebhookRequestRequestTypeDef,
-    GenerateAccessLogsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetAppRequestRequestTypeDef,
     GetArtifactUrlRequestRequestTypeDef,
     GetBackendEnvironmentRequestRequestTypeDef,
     GetBranchRequestRequestTypeDef,
     GetDomainAssociationRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetWebhookRequestRequestTypeDef,
@@ -338,23 +339,23 @@
     ListBackendEnvironmentsRequestRequestTypeDef,
     ListBranchesRequestRequestTypeDef,
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
+    AppTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
-    AppTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
     GenerateAccessLogsResultTypeDef,
     GetArtifactUrlResultTypeDef,
@@ -374,14 +375,16 @@
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
     ListJobsResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
+    GenerateAccessLogsRequestRequestTypeDef,
+    StartJobRequestRequestTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
@@ -394,15 +397,15 @@
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplify-2.5.2/setup.py` & `types-aiobotocore-amplify-2.5.2.post1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplify",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Amplify 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore amplify type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore amplify type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_amplify": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/"
```

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/__init__.py` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/__init__.pyi` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/__main__.py` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Amplify 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Amplify 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/client.py` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 
     session = get_session()
     async with session.create_client("amplify") as client:
         client: AmplifyClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import JobTypeType, PlatformType, StageType
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
     CustomRuleTypeDef,
@@ -59,14 +58,15 @@
     ListJobsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebhooksResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     SubDomainSettingTypeDef,
+    TimestampTypeDef,
     UpdateAppResultTypeDef,
     UpdateBranchResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
     UpdateWebhookResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -147,15 +147,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_app)
         """
@@ -296,16 +296,16 @@
         """
 
     async def generate_access_logs(
         self,
         *,
         domainName: str,
         appId: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> GenerateAccessLogsResultTypeDef:
         """
         Returns the website access logs for a specific time range using a presigned URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#generate_access_logs)
         """
@@ -486,15 +486,15 @@
         appId: str,
         branchName: str,
         jobType: JobTypeType,
         jobId: str = ...,
         jobReason: str = ...,
         commitId: str = ...,
         commitMessage: str = ...,
-        commitTime: Union[datetime, str] = ...
+        commitTime: TimestampTypeDef = ...
     ) -> StartJobResultTypeDef:
         """
         Starts a new job for a branch of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#start_job)
         """
@@ -537,15 +537,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/client.pyi` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 
     session = get_session()
     async with session.create_client("amplify") as client:
         client: AmplifyClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import JobTypeType, PlatformType, StageType
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
     CustomRuleTypeDef,
@@ -59,14 +58,15 @@
     ListJobsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebhooksResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     SubDomainSettingTypeDef,
+    TimestampTypeDef,
     UpdateAppResultTypeDef,
     UpdateBranchResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
     UpdateWebhookResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -140,15 +140,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_app)
         """
@@ -277,16 +277,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#delete_webhook)
         """
     async def generate_access_logs(
         self,
         *,
         domainName: str,
         appId: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> GenerateAccessLogsResultTypeDef:
         """
         Returns the website access logs for a specific time range using a presigned URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#generate_access_logs)
         """
@@ -449,15 +449,15 @@
         appId: str,
         branchName: str,
         jobType: JobTypeType,
         jobId: str = ...,
         jobReason: str = ...,
         commitId: str = ...,
         commitMessage: str = ...,
-        commitTime: Union[datetime, str] = ...
+        commitTime: TimestampTypeDef = ...
     ) -> StartJobResultTypeDef:
         """
         Starts a new job for a branch of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#start_job)
         """
@@ -496,15 +496,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/literals.py` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/literals.pyi` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/paginator.py` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/paginator.pyi` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/type_defs.py` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigTypeDef
+    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigTypeDef = {...}
+    data: AutoBranchCreationConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,18 +27,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AutoBranchCreationConfigTypeDef",
+    "AutoBranchCreationConfigOutputTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
@@ -47,15 +48,15 @@
     "DeleteAppRequestRequestTypeDef",
     "DeleteBackendEnvironmentRequestRequestTypeDef",
     "DeleteBranchRequestRequestTypeDef",
     "DeleteDomainAssociationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "JobSummaryTypeDef",
     "DeleteWebhookRequestRequestTypeDef",
-    "GenerateAccessLogsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetArtifactUrlRequestRequestTypeDef",
     "GetBackendEnvironmentRequestRequestTypeDef",
     "GetBranchRequestRequestTypeDef",
     "GetDomainAssociationRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetWebhookRequestRequestTypeDef",
@@ -66,23 +67,23 @@
     "ListBackendEnvironmentsRequestRequestTypeDef",
     "ListBranchesRequestRequestTypeDef",
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
+    "AppTypeDef",
+    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
-    "AppTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
     "GenerateAccessLogsResultTypeDef",
     "GetArtifactUrlResultTypeDef",
@@ -102,14 +103,16 @@
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
     "ListJobsResultTypeDef",
     "StartDeploymentResultTypeDef",
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
+    "GenerateAccessLogsRequestRequestTypeDef",
+    "StartJobRequestRequestTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
@@ -121,21 +124,21 @@
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
+AutoBranchCreationConfigOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigOutputTypeDef",
     {
         "stage": StageType,
         "framework": str,
         "enableAutoBuild": bool,
-        "environmentVariables": Mapping[str, str],
+        "environmentVariables": Dict[str, str],
         "basicAuthCredentials": str,
         "enableBasicAuth": bool,
         "enablePerformanceMode": bool,
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
@@ -178,14 +181,31 @@
     "ArtifactTypeDef",
     {
         "artifactFileName": str,
         "artifactId": str,
     },
 )
 
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
+    {
+        "stage": StageType,
+        "framework": str,
+        "enableAutoBuild": bool,
+        "environmentVariables": Mapping[str, str],
+        "basicAuthCredentials": str,
+        "enableBasicAuth": bool,
+        "enablePerformanceMode": bool,
+        "buildSpec": str,
+        "enablePullRequestPreview": bool,
+        "pullRequestEnvironmentName": str,
+    },
+    total=False,
+)
+
 _RequiredBackendEnvironmentTypeDef = TypedDict(
     "_RequiredBackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
         "createTime": datetime,
         "updateTime": datetime,
@@ -457,38 +477,15 @@
 DeleteWebhookRequestRequestTypeDef = TypedDict(
     "DeleteWebhookRequestRequestTypeDef",
     {
         "webhookId": str,
     },
 )
 
-_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "domainName": str,
-        "appId": str,
-    },
-)
-_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GenerateAccessLogsRequestRequestTypeDef(
-    _RequiredGenerateAccessLogsRequestRequestTypeDef,
-    _OptionalGenerateAccessLogsRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 GetAppRequestRequestTypeDef = TypedDict(
     "GetAppRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
@@ -750,41 +747,14 @@
 
 class StartDeploymentRequestRequestTypeDef(
     _RequiredStartDeploymentRequestRequestTypeDef, _OptionalStartDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartJobRequestRequestTypeDef",
-    {
-        "appId": str,
-        "branchName": str,
-        "jobType": JobTypeType,
-    },
-)
-_OptionalStartJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartJobRequestRequestTypeDef",
-    {
-        "jobId": str,
-        "jobReason": str,
-        "commitId": str,
-        "commitMessage": str,
-        "commitTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class StartJobRequestRequestTypeDef(
-    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
-):
-    pass
-
-
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
@@ -860,14 +830,58 @@
 
 class UpdateWebhookRequestRequestTypeDef(
     _RequiredUpdateWebhookRequestRequestTypeDef, _OptionalUpdateWebhookRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
+    {
+        "appId": str,
+        "appArn": str,
+        "name": str,
+        "description": str,
+        "repository": str,
+        "platform": PlatformType,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "environmentVariables": Dict[str, str],
+        "defaultDomain": str,
+        "enableBranchAutoBuild": bool,
+        "enableBasicAuth": bool,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "tags": Dict[str, str],
+        "iamServiceRoleArn": str,
+        "enableBranchAutoDeletion": bool,
+        "basicAuthCredentials": str,
+        "customRules": List[CustomRuleTypeDef],
+        "productionBranch": ProductionBranchTypeDef,
+        "buildSpec": str,
+        "customHeaders": str,
+        "enableAutoBranchCreation": bool,
+        "autoBranchCreationPatterns": List[str],
+        "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
+        "repositoryCloneMethod": RepositoryCloneMethodType,
+    },
+    total=False,
+)
+
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
+
+AutoBranchCreationConfigUnionTypeDef = Union[
+    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+]
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -936,55 +950,14 @@
 
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "tags": Dict[str, str],
-        "iamServiceRoleArn": str,
-        "enableBranchAutoDeletion": bool,
-        "basicAuthCredentials": str,
-        "customRules": List[CustomRuleTypeDef],
-        "productionBranch": ProductionBranchTypeDef,
-        "buildSpec": str,
-        "customHeaders": str,
-        "enableAutoBranchCreation": bool,
-        "autoBranchCreationPatterns": List[str],
-        "autoBranchCreationConfig": AutoBranchCreationConfigTypeDef,
-        "repositoryCloneMethod": RepositoryCloneMethodType,
-    },
-    total=False,
-)
-
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
-
 CreateBackendEnvironmentResultTypeDef = TypedDict(
     "CreateBackendEnvironmentResultTypeDef",
     {
         "backendEnvironment": BackendEnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1238,14 +1211,65 @@
     "StopJobResultTypeDef",
     {
         "jobSummary": JobSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "domainName": str,
+        "appId": str,
+    },
+)
+_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GenerateAccessLogsRequestRequestTypeDef(
+    _RequiredGenerateAccessLogsRequestRequestTypeDef,
+    _OptionalGenerateAccessLogsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "branchName": str,
+        "jobType": JobTypeType,
+    },
+)
+_OptionalStartJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartJobRequestRequestTypeDef",
+    {
+        "jobId": str,
+        "jobReason": str,
+        "commitId": str,
+        "commitMessage": str,
+        "commitTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class StartJobRequestRequestTypeDef(
+    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
+):
+    pass
+
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "summary": JobSummaryTypeDef,
         "steps": List[StepTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify/type_defs.pyi` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigTypeDef
+    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigTypeDef = {...}
+    data: AutoBranchCreationConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -26,18 +26,19 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AutoBranchCreationConfigTypeDef",
+    "AutoBranchCreationConfigOutputTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
@@ -46,15 +47,15 @@
     "DeleteAppRequestRequestTypeDef",
     "DeleteBackendEnvironmentRequestRequestTypeDef",
     "DeleteBranchRequestRequestTypeDef",
     "DeleteDomainAssociationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "JobSummaryTypeDef",
     "DeleteWebhookRequestRequestTypeDef",
-    "GenerateAccessLogsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetArtifactUrlRequestRequestTypeDef",
     "GetBackendEnvironmentRequestRequestTypeDef",
     "GetBranchRequestRequestTypeDef",
     "GetDomainAssociationRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetWebhookRequestRequestTypeDef",
@@ -65,23 +66,23 @@
     "ListBackendEnvironmentsRequestRequestTypeDef",
     "ListBranchesRequestRequestTypeDef",
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
+    "AppTypeDef",
+    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
-    "AppTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
     "GenerateAccessLogsResultTypeDef",
     "GetArtifactUrlResultTypeDef",
@@ -101,14 +102,16 @@
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
     "ListJobsResultTypeDef",
     "StartDeploymentResultTypeDef",
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
+    "GenerateAccessLogsRequestRequestTypeDef",
+    "StartJobRequestRequestTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
@@ -120,21 +123,21 @@
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
+AutoBranchCreationConfigOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigOutputTypeDef",
     {
         "stage": StageType,
         "framework": str,
         "enableAutoBuild": bool,
-        "environmentVariables": Mapping[str, str],
+        "environmentVariables": Dict[str, str],
         "basicAuthCredentials": str,
         "enableBasicAuth": bool,
         "enablePerformanceMode": bool,
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
@@ -175,14 +178,31 @@
     "ArtifactTypeDef",
     {
         "artifactFileName": str,
         "artifactId": str,
     },
 )
 
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
+    {
+        "stage": StageType,
+        "framework": str,
+        "enableAutoBuild": bool,
+        "environmentVariables": Mapping[str, str],
+        "basicAuthCredentials": str,
+        "enableBasicAuth": bool,
+        "enablePerformanceMode": bool,
+        "buildSpec": str,
+        "enablePullRequestPreview": bool,
+        "pullRequestEnvironmentName": str,
+    },
+    total=False,
+)
+
 _RequiredBackendEnvironmentTypeDef = TypedDict(
     "_RequiredBackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
         "createTime": datetime,
         "updateTime": datetime,
@@ -440,36 +460,15 @@
 DeleteWebhookRequestRequestTypeDef = TypedDict(
     "DeleteWebhookRequestRequestTypeDef",
     {
         "webhookId": str,
     },
 )
 
-_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "domainName": str,
-        "appId": str,
-    },
-)
-_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GenerateAccessLogsRequestRequestTypeDef(
-    _RequiredGenerateAccessLogsRequestRequestTypeDef,
-    _OptionalGenerateAccessLogsRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 GetAppRequestRequestTypeDef = TypedDict(
     "GetAppRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
@@ -715,39 +714,14 @@
 )
 
 class StartDeploymentRequestRequestTypeDef(
     _RequiredStartDeploymentRequestRequestTypeDef, _OptionalStartDeploymentRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartJobRequestRequestTypeDef",
-    {
-        "appId": str,
-        "branchName": str,
-        "jobType": JobTypeType,
-    },
-)
-_OptionalStartJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartJobRequestRequestTypeDef",
-    {
-        "jobId": str,
-        "jobReason": str,
-        "commitId": str,
-        "commitMessage": str,
-        "commitTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class StartJobRequestRequestTypeDef(
-    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
-):
-    pass
-
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
@@ -819,14 +793,56 @@
 )
 
 class UpdateWebhookRequestRequestTypeDef(
     _RequiredUpdateWebhookRequestRequestTypeDef, _OptionalUpdateWebhookRequestRequestTypeDef
 ):
     pass
 
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
+    {
+        "appId": str,
+        "appArn": str,
+        "name": str,
+        "description": str,
+        "repository": str,
+        "platform": PlatformType,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "environmentVariables": Dict[str, str],
+        "defaultDomain": str,
+        "enableBranchAutoBuild": bool,
+        "enableBasicAuth": bool,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "tags": Dict[str, str],
+        "iamServiceRoleArn": str,
+        "enableBranchAutoDeletion": bool,
+        "basicAuthCredentials": str,
+        "customRules": List[CustomRuleTypeDef],
+        "productionBranch": ProductionBranchTypeDef,
+        "buildSpec": str,
+        "customHeaders": str,
+        "enableAutoBranchCreation": bool,
+        "autoBranchCreationPatterns": List[str],
+        "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
+        "repositoryCloneMethod": RepositoryCloneMethodType,
+    },
+    total=False,
+)
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
+AutoBranchCreationConfigUnionTypeDef = Union[
+    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+]
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -891,53 +907,14 @@
 )
 
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "tags": Dict[str, str],
-        "iamServiceRoleArn": str,
-        "enableBranchAutoDeletion": bool,
-        "basicAuthCredentials": str,
-        "customRules": List[CustomRuleTypeDef],
-        "productionBranch": ProductionBranchTypeDef,
-        "buildSpec": str,
-        "customHeaders": str,
-        "enableAutoBranchCreation": bool,
-        "autoBranchCreationPatterns": List[str],
-        "autoBranchCreationConfig": AutoBranchCreationConfigTypeDef,
-        "repositoryCloneMethod": RepositoryCloneMethodType,
-    },
-    total=False,
-)
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
 CreateBackendEnvironmentResultTypeDef = TypedDict(
     "CreateBackendEnvironmentResultTypeDef",
     {
         "backendEnvironment": BackendEnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1187,14 +1164,61 @@
     "StopJobResultTypeDef",
     {
         "jobSummary": JobSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "domainName": str,
+        "appId": str,
+    },
+)
+_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GenerateAccessLogsRequestRequestTypeDef(
+    _RequiredGenerateAccessLogsRequestRequestTypeDef,
+    _OptionalGenerateAccessLogsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "branchName": str,
+        "jobType": JobTypeType,
+    },
+)
+_OptionalStartJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartJobRequestRequestTypeDef",
+    {
+        "jobId": str,
+        "jobReason": str,
+        "commitId": str,
+        "commitMessage": str,
+        "commitTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class StartJobRequestRequestTypeDef(
+    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
+):
+    pass
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "summary": JobSummaryTypeDef,
         "steps": List[StepTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/PKG-INFO` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplify
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Amplify 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Amplify 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore amplify type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore amplify type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amplify"></a>
 
 # types-aiobotocore-amplify
 
 [![PyPI - types-aiobotocore-amplify](https://img.shields.io/pypi/v/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplify?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplify)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplify)](https://pepy.tech/project/types-aiobotocore-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Amplify 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [types-aiobotocore-amplify docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/).
 
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
@@ -323,27 +322,28 @@
 )
 
 
 def check_value(value: DomainStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplify.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplify.type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigOutputTypeDef,
     CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
+    AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
@@ -352,15 +352,15 @@
     DeleteAppRequestRequestTypeDef,
     DeleteBackendEnvironmentRequestRequestTypeDef,
     DeleteBranchRequestRequestTypeDef,
     DeleteDomainAssociationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     JobSummaryTypeDef,
     DeleteWebhookRequestRequestTypeDef,
-    GenerateAccessLogsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetAppRequestRequestTypeDef,
     GetArtifactUrlRequestRequestTypeDef,
     GetBackendEnvironmentRequestRequestTypeDef,
     GetBranchRequestRequestTypeDef,
     GetDomainAssociationRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetWebhookRequestRequestTypeDef,
@@ -371,23 +371,23 @@
     ListBackendEnvironmentsRequestRequestTypeDef,
     ListBranchesRequestRequestTypeDef,
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
+    AppTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
-    AppTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
     GenerateAccessLogsResultTypeDef,
     GetArtifactUrlResultTypeDef,
@@ -407,14 +407,16 @@
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
     ListJobsResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
+    GenerateAccessLogsRequestRequestTypeDef,
+    StartJobRequestRequestTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
@@ -427,15 +429,15 @@
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplify-2.5.2/types_aiobotocore_amplify.egg-info/SOURCES.txt` & `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*


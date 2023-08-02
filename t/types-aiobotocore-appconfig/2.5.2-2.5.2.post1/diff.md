# Comparing `tmp/types-aiobotocore-appconfig-2.5.2.tar.gz` & `tmp/types-aiobotocore-appconfig-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfig-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfig-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-appconfig-2.5.2.tar` & `types-aiobotocore-appconfig-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.433654 types-aiobotocore-appconfig-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-08 01:43:12.433654 types-aiobotocore-appconfig-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.433654 types-aiobotocore-appconfig-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:25:39.000000 types-aiobotocore-appconfig-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.425654 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31219 2023-07-08 01:25:41.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31174 2023-07-08 01:25:41.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:40.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.433654 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-08 01:43:12.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-08 01:43:12.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:12.000000 types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.445660 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31152 2023-08-02 14:33:07.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-02 14:33:07.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfig-2.5.2/LICENSE` & `types-aiobotocore-appconfig-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2/PKG-INFO` & `types-aiobotocore-appconfig-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appconfig type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appconfig type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appconfig"></a>
 
 # types-aiobotocore-appconfig
 
 [![PyPI - types-aiobotocore-appconfig](https://img.shields.io/pypi/v/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfig?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfig)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
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
@@ -288,89 +287,90 @@
 )
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appconfig.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
+    BlobTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
-    ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExtensionAssociationSummaryTypeDef,
-    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
-    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagsTypeDef,
-    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
+    ApplicationResponseTypeDef,
+    ConfigurationTypeDef,
+    DeploymentStrategyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExtensionAssociationTypeDef,
+    HostedConfigurationVersionTypeDef,
+    ResourceTagsTypeDef,
     ApplicationsTypeDef,
+    CreateHostedConfigurationVersionRequestRequestTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
     ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
@@ -378,15 +378,15 @@
     ExtensionsTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
-def get_structure() -> ActionInvocationTypeDef:
+def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appconfig-2.5.2/README.md` & `types-aiobotocore-appconfig-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-appconfig"></a>
 
 # types-aiobotocore-appconfig
 
 [![PyPI - types-aiobotocore-appconfig](https://img.shields.io/pypi/v/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfig?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfig)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
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
@@ -255,89 +255,90 @@
 )
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appconfig.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
+    BlobTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
-    ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExtensionAssociationSummaryTypeDef,
-    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
-    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagsTypeDef,
-    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
+    ApplicationResponseTypeDef,
+    ConfigurationTypeDef,
+    DeploymentStrategyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExtensionAssociationTypeDef,
+    HostedConfigurationVersionTypeDef,
+    ResourceTagsTypeDef,
     ApplicationsTypeDef,
+    CreateHostedConfigurationVersionRequestRequestTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
     ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
@@ -345,15 +346,15 @@
     ExtensionsTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
-def get_structure() -> ActionInvocationTypeDef:
+def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appconfig-2.5.2/setup.py` & `types-aiobotocore-appconfig-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfig",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore appconfig type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore appconfig type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appconfig": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/"
```

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/__main__.py` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppConfig 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AppConfig 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/client.py` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,34 @@
     from types_aiobotocore_appconfig.client import AppConfigClient
 
     session = get_session()
     async with session.create_client("appconfig") as client:
         client: AppConfigClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import ActionPointType, GrowthTypeType, ReplicateToType
 from .type_defs import (
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ApplicationResponseTypeDef,
     ApplicationsTypeDef,
+    BlobTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     ConfigurationTypeDef,
     DeploymentStrategiesTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
+    DeploymentStrategyResponseTypeDef,
     DeploymentsTypeDef,
     DeploymentTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentsTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionsTypeDef,
     ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     HostedConfigurationVersionTypeDef,
@@ -99,15 +99,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#close)
         """
 
     async def create_application(
         self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_application)
         """
 
@@ -138,15 +138,15 @@
         DeploymentDurationInMinutes: int,
         GrowthFactor: float,
         Description: str = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthType: GrowthTypeType = ...,
         ReplicateTo: ReplicateToType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Creates a deployment strategy that defines important criteria for rolling out
         your configuration to the designated targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_deployment_strategy)
         """
@@ -155,15 +155,15 @@
         self,
         *,
         ApplicationId: str,
         Name: str,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Creates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_environment)
         """
 
@@ -203,15 +203,15 @@
         """
 
     async def create_hosted_configuration_version(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
-        Content: Union[str, bytes, IO[Any], StreamingBody],
+        Content: BlobTypeDef,
         ContentType: str,
         Description: str = ...,
         LatestVersionNumber: int = ...,
         VersionLabel: str = ...
     ) -> HostedConfigurationVersionTypeDef:
         """
         Creates a new configuration in the AppConfig hosted configuration store.
@@ -299,15 +299,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#generate_presigned_url)
         """
 
-    async def get_application(self, *, ApplicationId: str) -> ApplicationResponseMetadataTypeDef:
+    async def get_application(self, *, ApplicationId: str) -> ApplicationResponseTypeDef:
         """
         Retrieves information about an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_application)
         """
 
@@ -345,25 +345,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_deployment)
         """
 
     async def get_deployment_strategy(
         self, *, DeploymentStrategyId: str
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Retrieves information about a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_deployment_strategy)
         """
 
     async def get_environment(
         self, *, ApplicationId: str, EnvironmentId: str
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Retrieves information about an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_environment)
         """
 
@@ -546,15 +546,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#untag_resource)
         """
 
     async def update_application(
         self, *, ApplicationId: str, Name: str = ..., Description: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_application)
         """
 
@@ -580,15 +580,15 @@
         *,
         DeploymentStrategyId: str,
         Description: str = ...,
         DeploymentDurationInMinutes: int = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthFactor: float = ...,
         GrowthType: GrowthTypeType = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Updates a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_deployment_strategy)
         """
 
@@ -596,15 +596,15 @@
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
         Name: str = ...,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/client.pyi` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,34 +10,34 @@
     from types_aiobotocore_appconfig.client import AppConfigClient
 
     session = get_session()
     async with session.create_client("appconfig") as client:
         client: AppConfigClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import ActionPointType, GrowthTypeType, ReplicateToType
 from .type_defs import (
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ApplicationResponseTypeDef,
     ApplicationsTypeDef,
+    BlobTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     ConfigurationTypeDef,
     DeploymentStrategiesTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
+    DeploymentStrategyResponseTypeDef,
     DeploymentsTypeDef,
     DeploymentTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentsTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionsTypeDef,
     ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     HostedConfigurationVersionTypeDef,
@@ -93,15 +93,15 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#close)
         """
     async def create_application(
         self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_application)
         """
     async def create_configuration_profile(
@@ -130,15 +130,15 @@
         DeploymentDurationInMinutes: int,
         GrowthFactor: float,
         Description: str = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthType: GrowthTypeType = ...,
         ReplicateTo: ReplicateToType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Creates a deployment strategy that defines important criteria for rolling out
         your configuration to the designated targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_deployment_strategy)
         """
@@ -146,15 +146,15 @@
         self,
         *,
         ApplicationId: str,
         Name: str,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Creates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_environment)
         """
     async def create_extension(
@@ -191,15 +191,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_extension_association)
         """
     async def create_hosted_configuration_version(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
-        Content: Union[str, bytes, IO[Any], StreamingBody],
+        Content: BlobTypeDef,
         ContentType: str,
         Description: str = ...,
         LatestVersionNumber: int = ...,
         VersionLabel: str = ...
     ) -> HostedConfigurationVersionTypeDef:
         """
         Creates a new configuration in the AppConfig hosted configuration store.
@@ -278,15 +278,15 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#generate_presigned_url)
         """
-    async def get_application(self, *, ApplicationId: str) -> ApplicationResponseMetadataTypeDef:
+    async def get_application(self, *, ApplicationId: str) -> ApplicationResponseTypeDef:
         """
         Retrieves information about an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_application)
         """
     async def get_configuration(
@@ -320,24 +320,24 @@
         Retrieves information about a configuration deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_deployment)
         """
     async def get_deployment_strategy(
         self, *, DeploymentStrategyId: str
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Retrieves information about a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_deployment_strategy)
         """
     async def get_environment(
         self, *, ApplicationId: str, EnvironmentId: str
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Retrieves information about an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_environment)
         """
     async def get_extension(
@@ -503,15 +503,15 @@
         Deletes a tag key and value from an AppConfig resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#untag_resource)
         """
     async def update_application(
         self, *, ApplicationId: str, Name: str = ..., Description: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_application)
         """
     async def update_configuration_profile(
@@ -535,30 +535,30 @@
         *,
         DeploymentStrategyId: str,
         Description: str = ...,
         DeploymentDurationInMinutes: int = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthFactor: float = ...,
         GrowthType: GrowthTypeType = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Updates a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_deployment_strategy)
         """
     async def update_environment(
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
         Name: str = ...,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_environment)
         """
     async def update_extension(
```

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/literals.py` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/literals.pyi` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/type_defs.py` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appconfig.type_defs import ActionInvocationTypeDef
 
-    data: ActionInvocationTypeDef = {...}
+    data: ActionInvocationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,78 +33,79 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
-    "ApplicationResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
+    "BlobTypeDef",
     "ConfigurationProfileSummaryTypeDef",
     "ValidatorTypeDef",
-    "ConfigurationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
-    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
-    "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExtensionAssociationSummaryTypeDef",
-    "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
     "GetExtensionRequestRequestTypeDef",
     "GetHostedConfigurationVersionRequestRequestTypeDef",
     "HostedConfigurationVersionSummaryTypeDef",
-    "HostedConfigurationVersionTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListConfigurationProfilesRequestRequestTypeDef",
     "ListDeploymentStrategiesRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListExtensionAssociationsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListHostedConfigurationVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResourceTagsTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateDeploymentStrategyRequestRequestTypeDef",
     "UpdateExtensionAssociationRequestRequestTypeDef",
     "ValidateConfigurationRequestRequestTypeDef",
     "DeploymentEventTypeDef",
+    "ApplicationResponseTypeDef",
+    "ConfigurationTypeDef",
+    "DeploymentStrategyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExtensionAssociationTypeDef",
+    "HostedConfigurationVersionTypeDef",
+    "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
+    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "EnvironmentResponseMetadataTypeDef",
+    "EnvironmentResponseTypeDef",
     "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateExtensionRequestRequestTypeDef",
     "ExtensionTypeDef",
     "UpdateExtensionRequestRequestTypeDef",
     "DeploymentStrategiesTypeDef",
     "DeploymentsTypeDef",
@@ -136,21 +137,22 @@
         "Description": str,
         "Uri": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Id": str,
@@ -167,14 +169,15 @@
         "ExtensionAssociationId": str,
         "VersionNumber": int,
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConfigurationProfileSummaryTypeDef = TypedDict(
     "ConfigurationProfileSummaryTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "LocationUri": str,
@@ -188,24 +191,14 @@
     "ValidatorTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Content": StreamingBody,
-        "ConfigurationVersion": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
@@ -301,41 +294,14 @@
     {
         "Description": str,
         "Required": bool,
     },
     total=False,
 )
 
-_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LatestVersionNumber": int,
-        "VersionLabel": str,
-    },
-    total=False,
-)
-
-
-class CreateHostedConfigurationVersionRequestRequestTypeDef(
-    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
-    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
-):
-    pass
-
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -410,29 +376,14 @@
         "GrowthFactor": float,
         "FinalBakeTimeInMinutes": int,
         "ReplicateTo": ReplicateToType,
     },
     total=False,
 )
 
-DeploymentStrategyResponseMetadataTypeDef = TypedDict(
-    "DeploymentStrategyResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "DeploymentDurationInMinutes": int,
-        "GrowthType": GrowthTypeType,
-        "GrowthFactor": float,
-        "FinalBakeTimeInMinutes": int,
-        "ReplicateTo": ReplicateToType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentSummaryTypeDef = TypedDict(
     "DeploymentSummaryTypeDef",
     {
         "DeploymentNumber": int,
         "ConfigurationName": str,
         "ConfigurationVersion": str,
         "DeploymentDurationInMinutes": int,
@@ -443,44 +394,24 @@
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
-ExtensionAssociationTypeDef = TypedDict(
-    "ExtensionAssociationTypeDef",
-    {
-        "Id": str,
-        "ExtensionArn": str,
-        "ResourceArn": str,
-        "Arn": str,
-        "Parameters": Dict[str, str],
-        "ExtensionVersionNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionSummaryTypeDef = TypedDict(
     "ExtensionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
@@ -598,28 +529,14 @@
         "Description": str,
         "ContentType": str,
         "VersionLabel": str,
     },
     total=False,
 )
 
-HostedConfigurationVersionTypeDef = TypedDict(
-    "HostedConfigurationVersionTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "VersionNumber": int,
-        "Description": str,
-        "Content": StreamingBody,
-        "ContentType": str,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -753,33 +670,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ResourceTagsTypeDef = TypedDict(
-    "ResourceTagsTypeDef",
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
 _RequiredStartDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDeploymentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
         "DeploymentStrategyId": str,
         "ConfigurationProfileId": str,
@@ -915,44 +813,148 @@
         "Description": str,
         "ActionInvocations": List[ActionInvocationTypeDef],
         "OccurredAt": datetime,
     },
     total=False,
 )
 
+ApplicationResponseTypeDef = TypedDict(
+    "ApplicationResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Content": StreamingBody,
+        "ConfigurationVersion": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeploymentStrategyResponseTypeDef = TypedDict(
+    "DeploymentStrategyResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "DeploymentDurationInMinutes": int,
+        "GrowthType": GrowthTypeType,
+        "GrowthFactor": float,
+        "FinalBakeTimeInMinutes": int,
+        "ReplicateTo": ReplicateToType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExtensionAssociationTypeDef = TypedDict(
+    "ExtensionAssociationTypeDef",
+    {
+        "Id": str,
+        "ExtensionArn": str,
+        "ResourceArn": str,
+        "Arn": str,
+        "Parameters": Dict[str, str],
+        "ExtensionVersionNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HostedConfigurationVersionTypeDef = TypedDict(
+    "HostedConfigurationVersionTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "VersionNumber": int,
+        "Description": str,
+        "Content": StreamingBody,
+        "ContentType": str,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResourceTagsTypeDef = TypedDict(
+    "ResourceTagsTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplicationsTypeDef = TypedDict(
     "ApplicationsTypeDef",
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "Content": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LatestVersionNumber": int,
+        "VersionLabel": str,
+    },
+    total=False,
+)
+
+
+class CreateHostedConfigurationVersionRequestRequestTypeDef(
+    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
+    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
+):
+    pass
+
+
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationProfileTypeDef = TypedDict(
     "ConfigurationProfileTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
         "Validators": List[ValidatorTypeDef],
         "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -1026,24 +1028,24 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
-EnvironmentResponseMetadataTypeDef = TypedDict(
-    "EnvironmentResponseMetadataTypeDef",
+EnvironmentResponseTypeDef = TypedDict(
+    "EnvironmentResponseTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "State": EnvironmentStateType,
         "Monitors": List[MonitorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "ApplicationId": str,
@@ -1111,15 +1113,15 @@
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
         "Actions": Dict[ActionPointType, List[ActionTypeDef]],
         "Parameters": Dict[str, ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
@@ -1144,51 +1146,51 @@
 
 
 DeploymentStrategiesTypeDef = TypedDict(
     "DeploymentStrategiesTypeDef",
     {
         "Items": List[DeploymentStrategyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtensionsTypeDef = TypedDict(
     "ExtensionsTypeDef",
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "ApplicationId": str,
@@ -1208,19 +1210,19 @@
         "EventLog": List[DeploymentEventTypeDef],
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
         "AppliedExtensions": List[AppliedExtensionTypeDef],
         "KmsKeyArn": str,
         "KmsKeyIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentsTypeDef = TypedDict(
     "EnvironmentsTypeDef",
     {
         "Items": List[EnvironmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig/type_defs.pyi` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appconfig.type_defs import ActionInvocationTypeDef
 
-    data: ActionInvocationTypeDef = {...}
+    data: ActionInvocationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -32,78 +32,79 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
-    "ApplicationResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
+    "BlobTypeDef",
     "ConfigurationProfileSummaryTypeDef",
     "ValidatorTypeDef",
-    "ConfigurationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
-    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
-    "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExtensionAssociationSummaryTypeDef",
-    "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
     "GetExtensionRequestRequestTypeDef",
     "GetHostedConfigurationVersionRequestRequestTypeDef",
     "HostedConfigurationVersionSummaryTypeDef",
-    "HostedConfigurationVersionTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListConfigurationProfilesRequestRequestTypeDef",
     "ListDeploymentStrategiesRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListExtensionAssociationsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListHostedConfigurationVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResourceTagsTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateDeploymentStrategyRequestRequestTypeDef",
     "UpdateExtensionAssociationRequestRequestTypeDef",
     "ValidateConfigurationRequestRequestTypeDef",
     "DeploymentEventTypeDef",
+    "ApplicationResponseTypeDef",
+    "ConfigurationTypeDef",
+    "DeploymentStrategyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExtensionAssociationTypeDef",
+    "HostedConfigurationVersionTypeDef",
+    "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
+    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "EnvironmentResponseMetadataTypeDef",
+    "EnvironmentResponseTypeDef",
     "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateExtensionRequestRequestTypeDef",
     "ExtensionTypeDef",
     "UpdateExtensionRequestRequestTypeDef",
     "DeploymentStrategiesTypeDef",
     "DeploymentsTypeDef",
@@ -135,21 +136,22 @@
         "Description": str,
         "Uri": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Id": str,
@@ -166,14 +168,15 @@
         "ExtensionAssociationId": str,
         "VersionNumber": int,
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConfigurationProfileSummaryTypeDef = TypedDict(
     "ConfigurationProfileSummaryTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "LocationUri": str,
@@ -187,24 +190,14 @@
     "ValidatorTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Content": StreamingBody,
-        "ConfigurationVersion": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
@@ -292,39 +285,14 @@
     {
         "Description": str,
         "Required": bool,
     },
     total=False,
 )
 
-_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LatestVersionNumber": int,
-        "VersionLabel": str,
-    },
-    total=False,
-)
-
-class CreateHostedConfigurationVersionRequestRequestTypeDef(
-    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
-    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
-):
-    pass
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -397,29 +365,14 @@
         "GrowthFactor": float,
         "FinalBakeTimeInMinutes": int,
         "ReplicateTo": ReplicateToType,
     },
     total=False,
 )
 
-DeploymentStrategyResponseMetadataTypeDef = TypedDict(
-    "DeploymentStrategyResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "DeploymentDurationInMinutes": int,
-        "GrowthType": GrowthTypeType,
-        "GrowthFactor": float,
-        "FinalBakeTimeInMinutes": int,
-        "ReplicateTo": ReplicateToType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentSummaryTypeDef = TypedDict(
     "DeploymentSummaryTypeDef",
     {
         "DeploymentNumber": int,
         "ConfigurationName": str,
         "ConfigurationVersion": str,
         "DeploymentDurationInMinutes": int,
@@ -430,44 +383,24 @@
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
-ExtensionAssociationTypeDef = TypedDict(
-    "ExtensionAssociationTypeDef",
-    {
-        "Id": str,
-        "ExtensionArn": str,
-        "ResourceArn": str,
-        "Arn": str,
-        "Parameters": Dict[str, str],
-        "ExtensionVersionNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionSummaryTypeDef = TypedDict(
     "ExtensionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
@@ -581,28 +514,14 @@
         "Description": str,
         "ContentType": str,
         "VersionLabel": str,
     },
     total=False,
 )
 
-HostedConfigurationVersionTypeDef = TypedDict(
-    "HostedConfigurationVersionTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "VersionNumber": int,
-        "Description": str,
-        "Content": StreamingBody,
-        "ContentType": str,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -728,33 +647,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ResourceTagsTypeDef = TypedDict(
-    "ResourceTagsTypeDef",
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
 _RequiredStartDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDeploymentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
         "DeploymentStrategyId": str,
         "ConfigurationProfileId": str,
@@ -882,44 +782,146 @@
         "Description": str,
         "ActionInvocations": List[ActionInvocationTypeDef],
         "OccurredAt": datetime,
     },
     total=False,
 )
 
+ApplicationResponseTypeDef = TypedDict(
+    "ApplicationResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Content": StreamingBody,
+        "ConfigurationVersion": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeploymentStrategyResponseTypeDef = TypedDict(
+    "DeploymentStrategyResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "DeploymentDurationInMinutes": int,
+        "GrowthType": GrowthTypeType,
+        "GrowthFactor": float,
+        "FinalBakeTimeInMinutes": int,
+        "ReplicateTo": ReplicateToType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExtensionAssociationTypeDef = TypedDict(
+    "ExtensionAssociationTypeDef",
+    {
+        "Id": str,
+        "ExtensionArn": str,
+        "ResourceArn": str,
+        "Arn": str,
+        "Parameters": Dict[str, str],
+        "ExtensionVersionNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HostedConfigurationVersionTypeDef = TypedDict(
+    "HostedConfigurationVersionTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "VersionNumber": int,
+        "Description": str,
+        "Content": StreamingBody,
+        "ContentType": str,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResourceTagsTypeDef = TypedDict(
+    "ResourceTagsTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplicationsTypeDef = TypedDict(
     "ApplicationsTypeDef",
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "Content": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LatestVersionNumber": int,
+        "VersionLabel": str,
     },
+    total=False,
 )
 
+class CreateHostedConfigurationVersionRequestRequestTypeDef(
+    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
+    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
+):
+    pass
+
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationProfileTypeDef = TypedDict(
     "ConfigurationProfileTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
         "Validators": List[ValidatorTypeDef],
         "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -987,24 +989,24 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-EnvironmentResponseMetadataTypeDef = TypedDict(
-    "EnvironmentResponseMetadataTypeDef",
+EnvironmentResponseTypeDef = TypedDict(
+    "EnvironmentResponseTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "State": EnvironmentStateType,
         "Monitors": List[MonitorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "ApplicationId": str,
@@ -1068,15 +1070,15 @@
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
         "Actions": Dict[ActionPointType, List[ActionTypeDef]],
         "Parameters": Dict[str, ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
@@ -1099,51 +1101,51 @@
     pass
 
 DeploymentStrategiesTypeDef = TypedDict(
     "DeploymentStrategiesTypeDef",
     {
         "Items": List[DeploymentStrategyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtensionsTypeDef = TypedDict(
     "ExtensionsTypeDef",
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "ApplicationId": str,
@@ -1163,19 +1165,19 @@
         "EventLog": List[DeploymentEventTypeDef],
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
         "AppliedExtensions": List[AppliedExtensionTypeDef],
         "KmsKeyArn": str,
         "KmsKeyIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentsTypeDef = TypedDict(
     "EnvironmentsTypeDef",
     {
         "Items": List[EnvironmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/PKG-INFO` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appconfig type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appconfig type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appconfig"></a>
 
 # types-aiobotocore-appconfig
 
 [![PyPI - types-aiobotocore-appconfig](https://img.shields.io/pypi/v/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfig?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfig)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
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
@@ -288,89 +287,90 @@
 )
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appconfig.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
+    BlobTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
-    ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExtensionAssociationSummaryTypeDef,
-    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
-    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagsTypeDef,
-    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
+    ApplicationResponseTypeDef,
+    ConfigurationTypeDef,
+    DeploymentStrategyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExtensionAssociationTypeDef,
+    HostedConfigurationVersionTypeDef,
+    ResourceTagsTypeDef,
     ApplicationsTypeDef,
+    CreateHostedConfigurationVersionRequestRequestTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
     ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
@@ -378,15 +378,15 @@
     ExtensionsTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
-def get_structure() -> ActionInvocationTypeDef:
+def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appconfig-2.5.2/types_aiobotocore_appconfig.egg-info/SOURCES.txt` & `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*


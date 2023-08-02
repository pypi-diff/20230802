# Comparing `tmp/types-aiobotocore-sms-2.5.2.tar.gz` & `tmp/types-aiobotocore-sms-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sms-2.5.2.tar", last modified: Sat Jul  8 01:44:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-sms-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
```

## Comparing `types-aiobotocore-sms-2.5.2.tar` & `types-aiobotocore-sms-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.590910 types-aiobotocore-sms-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-07-08 01:44:20.590910 types-aiobotocore-sms-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:20.590910 types-aiobotocore-sms-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.590910 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27758 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-07-08 01:41:12.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28507 2023-07-08 01:41:12.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:11.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.590910 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-07-08 01:44:20.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:20.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:20.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:20.000000 types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31311 2023-08-02 14:49:52.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31295 2023-08-02 14:49:49.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sms-2.5.2/LICENSE` & `types-aiobotocore-sms-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2/PKG-INFO` & `types-aiobotocore-sms-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sms"></a>
 
 # types-aiobotocore-sms
 
 [![PyPI - types-aiobotocore-sms](https://img.shields.io/pypi/v/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sms?color=blue)](https://pypistats.org/packages/types-aiobotocore-sms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms)](https://pepy.tech/project/types-aiobotocore-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
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
@@ -340,112 +339,123 @@
 )
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
-    CreateReplicationJobResponseTypeDef,
+    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
     S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
-    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    ServerReplicationParametersTypeDef,
+    ServerReplicationParametersOutputTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
+    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
+    CreateReplicationJobRequestRequestTypeDef,
+    ServerReplicationParametersTypeDef,
+    UpdateReplicationJobRequestRequestTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
     ServerTypeDef,
     ReplicationJobTypeDef,
     AppValidationConfigurationTypeDef,
     GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
     ServerReplicationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
     ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
-    CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
-    UpdateAppRequestRequestTypeDef,
     UpdateAppResponseTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupLaunchConfigurationOutputTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
+    ServerGroupReplicationConfigurationOutputTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
+    ServerGroupValidationConfigurationOutputTypeDef,
     ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     GetAppValidationOutputResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LaunchDetailsTypeDef:
+def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sms-2.5.2/README.md` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-sms
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore sms type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-sms"></a>
 
 # types-aiobotocore-sms
 
 [![PyPI - types-aiobotocore-sms](https://img.shields.io/pypi/v/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sms?color=blue)](https://pypistats.org/packages/types-aiobotocore-sms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms)](https://pepy.tech/project/types-aiobotocore-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -307,112 +339,123 @@
 )
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
-    CreateReplicationJobResponseTypeDef,
+    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
     S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
-    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    ServerReplicationParametersTypeDef,
+    ServerReplicationParametersOutputTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
+    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
+    CreateReplicationJobRequestRequestTypeDef,
+    ServerReplicationParametersTypeDef,
+    UpdateReplicationJobRequestRequestTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
     ServerTypeDef,
     ReplicationJobTypeDef,
     AppValidationConfigurationTypeDef,
     GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
     ServerReplicationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
     ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
-    CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
-    UpdateAppRequestRequestTypeDef,
     UpdateAppResponseTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupLaunchConfigurationOutputTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
+    ServerGroupReplicationConfigurationOutputTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
+    ServerGroupValidationConfigurationOutputTypeDef,
     ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     GetAppValidationOutputResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LaunchDetailsTypeDef:
+def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sms-2.5.2/setup.py` & `types-aiobotocore-sms-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sms",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore sms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/__init__.py` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/__init__.pyi` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/__main__.py` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SMS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SMS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
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

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/client.py` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("sms") as client:
         client: SMSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import LicenseTypeType, OutputFormatType
 from .paginator import (
     GetConnectorsPaginator,
@@ -42,20 +41,21 @@
     GetAppValidationOutputResponseTypeDef,
     GetConnectorsResponseTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     GetServersResponseTypeDef,
     ListAppsResponseTypeDef,
     NotificationContextTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     VmServerAddressTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -125,29 +125,29 @@
     async def create_app(
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
-        serverGroups: Sequence[ServerGroupTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_app)
         """
 
     async def create_replication_job(
         self,
         *,
         serverId: str,
-        seedReplicationTime: Union[datetime, str],
+        seedReplicationTime: TimestampTypeDef,
         frequency: int = ...,
         runOnce: bool = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
@@ -399,29 +399,29 @@
 
     async def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_launch_configuration)
         """
 
     async def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
-            ServerGroupReplicationConfigurationTypeDef
+            ServerGroupReplicationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_replication_configuration)
@@ -429,15 +429,15 @@
 
     async def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
-            ServerGroupValidationConfigurationTypeDef
+            ServerGroupValidationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_validation_configuration)
@@ -492,30 +492,30 @@
     async def update_app(
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
-        serverGroups: Sequence[ServerGroupTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_app)
         """
 
     async def update_replication_job(
         self,
         *,
         replicationJobId: str,
         frequency: int = ...,
-        nextReplicationRunStartTime: Union[datetime, str] = ...,
+        nextReplicationRunStartTime: TimestampTypeDef = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
         kmsKeyId: str = ...
     ) -> Dict[str, Any]:
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/client.pyi` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("sms") as client:
         client: SMSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import LicenseTypeType, OutputFormatType
 from .paginator import (
     GetConnectorsPaginator,
@@ -42,20 +41,21 @@
     GetAppValidationOutputResponseTypeDef,
     GetConnectorsResponseTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     GetServersResponseTypeDef,
     ListAppsResponseTypeDef,
     NotificationContextTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     VmServerAddressTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -118,28 +118,28 @@
     async def create_app(
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
-        serverGroups: Sequence[ServerGroupTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_app)
         """
     async def create_replication_job(
         self,
         *,
         serverId: str,
-        seedReplicationTime: Union[datetime, str],
+        seedReplicationTime: TimestampTypeDef,
         frequency: int = ...,
         runOnce: bool = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
@@ -366,43 +366,43 @@
         """
     async def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_launch_configuration)
         """
     async def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
-            ServerGroupReplicationConfigurationTypeDef
+            ServerGroupReplicationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_replication_configuration)
         """
     async def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
-            ServerGroupValidationConfigurationTypeDef
+            ServerGroupValidationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_validation_configuration)
@@ -451,29 +451,29 @@
     async def update_app(
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
-        serverGroups: Sequence[ServerGroupTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_app)
         """
     async def update_replication_job(
         self,
         *,
         replicationJobId: str,
         frequency: int = ...,
-        nextReplicationRunStartTime: Union[datetime, str] = ...,
+        nextReplicationRunStartTime: TimestampTypeDef = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
         kmsKeyId: str = ...
     ) -> Dict[str, Any]:
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/literals.py` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/literals.pyi` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/paginator.py` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,45 +65,45 @@
 class GetConnectorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getconnectorspaginator)
         """
 
 
 class GetReplicationJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationjobspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReplicationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationjobspaginator)
         """
 
 
 class GetReplicationRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationrunspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReplicationRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationrunspaginator)
         """
 
 
@@ -113,28 +113,28 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
         """
 
 
 class ListAppsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#listappspaginator)
     """
 
     def paginate(
-        self, *, appIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#listappspaginator)
         """
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/paginator.pyi` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,43 +62,43 @@
 class GetConnectorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getconnectorspaginator)
         """
 
 class GetReplicationJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationjobspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReplicationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationjobspaginator)
         """
 
 class GetReplicationRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationrunspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReplicationRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getreplicationrunspaginator)
         """
 
 class GetServersPaginator(AioPaginator):
@@ -107,27 +107,27 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
         """
 
 class ListAppsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#listappspaginator)
     """
 
     def paginate(
-        self, *, appIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#listappspaginator)
         """
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/type_defs.py` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sms.type_defs import LaunchDetailsTypeDef
 
-    data: LaunchDetailsTypeDef = {...}
+    data: LaunchDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,101 +39,111 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
-    "CreateReplicationJobRequestRequestTypeDef",
-    "CreateReplicationJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
     "S3LocationTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetConnectorsRequestRequestTypeDef",
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationJobsRequestRequestTypeDef",
-    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
-    "ListAppsRequestListAppsPaginateTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
-    "PaginatorConfigTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "ResponseMetadataTypeDef",
-    "ServerReplicationParametersTypeDef",
+    "ServerReplicationParametersOutputTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
-    "StartOnDemandReplicationRunResponseTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
-    "UpdateReplicationJobRequestRequestTypeDef",
     "AppSummaryTypeDef",
+    "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
+    "StartOnDemandReplicationRunResponseTypeDef",
+    "CreateReplicationJobRequestRequestTypeDef",
+    "ServerReplicationParametersTypeDef",
+    "UpdateReplicationJobRequestRequestTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
     "ServerTypeDef",
     "ReplicationJobTypeDef",
     "AppValidationConfigurationTypeDef",
     "GetServersResponseTypeDef",
+    "ServerGroupOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
+    "ServerReplicationConfigurationOutputTypeDef",
     "ServerReplicationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
     "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
-    "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "UpdateAppResponseTypeDef",
+    "ServerGroupUnionTypeDef",
+    "ServerGroupLaunchConfigurationOutputTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
+    "ServerGroupReplicationConfigurationOutputTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
+    "ServerGroupValidationConfigurationOutputTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "ServerGroupLaunchConfigurationUnionTypeDef",
     "GetAppReplicationConfigurationResponseTypeDef",
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "ServerGroupReplicationConfigurationUnionTypeDef",
     "GetAppValidationConfigurationResponseTypeDef",
-    "PutAppValidationConfigurationRequestRequestTypeDef",
+    "ServerGroupValidationConfigurationUnionTypeDef",
     "GetAppValidationOutputResponseTypeDef",
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "PutAppValidationConfigurationRequestRequestTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
         "stackName": str,
@@ -164,52 +174,26 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReplicationJobRequestRequestTypeDef",
-    {
-        "serverId": str,
-        "seedReplicationTime": Union[datetime, str],
-    },
-)
-_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class CreateReplicationJobRequestRequestTypeDef(
-    _RequiredCreateReplicationJobRequestRequestTypeDef,
-    _OptionalCreateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
-
-CreateReplicationJobResponseTypeDef = TypedDict(
-    "CreateReplicationJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "replicationJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -314,72 +298,43 @@
 GetAppValidationOutputRequestRequestTypeDef = TypedDict(
     "GetAppValidationOutputRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
-GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetConnectorsRequestRequestTypeDef = TypedDict(
     "GetConnectorsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetReplicationJobsRequestRequestTypeDef = TypedDict(
     "GetReplicationJobsRequestRequestTypeDef",
     {
         "replicationJobId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
-    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReplicationRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetReplicationRunsRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalGetReplicationRunsRequestRequestTypeDef = TypedDict(
@@ -387,22 +342,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetReplicationRunsRequestRequestTypeDef(
     _RequiredGetReplicationRunsRequestRequestTypeDef,
     _OptionalGetReplicationRunsRequestRequestTypeDef,
 ):
     pass
 
-
 VmServerAddressTypeDef = TypedDict(
     "VmServerAddressTypeDef",
     {
         "vmManagerId": str,
         "vmId": str,
     },
     total=False,
@@ -420,23 +373,14 @@
     "LaunchAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-ListAppsRequestListAppsPaginateTypeDef = TypedDict(
-    "ListAppsRequestListAppsPaginateTypeDef",
-    {
-        "appIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -449,46 +393,25 @@
         "validationId": str,
         "status": ValidationStatusType,
         "statusMessage": str,
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
 ReplicationRunStageDetailsTypeDef = TypedDict(
     "ReplicationRunStageDetailsTypeDef",
     {
         "stage": str,
         "stageProgress": str,
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
-ServerReplicationParametersTypeDef = TypedDict(
-    "ServerReplicationParametersTypeDef",
+ServerReplicationParametersOutputTypeDef = TypedDict(
+    "ServerReplicationParametersOutputTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
@@ -515,52 +438,40 @@
     "_OptionalStartOnDemandAppReplicationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class StartOnDemandAppReplicationRequestRequestTypeDef(
     _RequiredStartOnDemandAppReplicationRequestRequestTypeDef,
     _OptionalStartOnDemandAppReplicationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
-
-StartOnDemandReplicationRunResponseTypeDef = TypedDict(
-    "StartOnDemandReplicationRunResponseTypeDef",
-    {
-        "replicationRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -569,43 +480,14 @@
     "TerminateAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "nextReplicationRunStartTime": Union[datetime, str],
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class UpdateReplicationJobRequestRequestTypeDef(
-    _RequiredUpdateReplicationJobRequestRequestTypeDef,
-    _OptionalUpdateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
-
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -624,36 +506,121 @@
         "roleName": str,
         "totalServerGroups": int,
         "totalServers": int,
     },
     total=False,
 )
 
+CreateReplicationJobResponseTypeDef = TypedDict(
+    "CreateReplicationJobResponseTypeDef",
+    {
+        "replicationJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetConnectorsResponseTypeDef = TypedDict(
     "GetConnectorsResponseTypeDef",
     {
         "connectorList": List[ConnectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandReplicationRunResponseTypeDef = TypedDict(
+    "StartOnDemandReplicationRunResponseTypeDef",
+    {
+        "replicationRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationJobRequestRequestTypeDef",
+    {
+        "serverId": str,
+        "seedReplicationTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+class CreateReplicationJobRequestRequestTypeDef(
+    _RequiredCreateReplicationJobRequestRequestTypeDef,
+    _OptionalCreateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
+ServerReplicationParametersTypeDef = TypedDict(
+    "ServerReplicationParametersTypeDef",
+    {
+        "seedTime": TimestampTypeDef,
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
     },
+    total=False,
 )
 
+_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "nextReplicationRunStartTime": TimestampTypeDef,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+class UpdateReplicationJobRequestRequestTypeDef(
+    _RequiredUpdateReplicationJobRequestRequestTypeDef,
+    _OptionalUpdateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
         "s3Location": S3LocationTypeDef,
@@ -673,19 +640,65 @@
     "UserDataTypeDef",
     {
         "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
+GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
+    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+):
+    pass
+
+ListAppsRequestListAppsPaginateTypeDef = TypedDict(
+    "ListAppsRequestListAppsPaginateTypeDef",
+    {
+        "appIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetServersRequestGetServersPaginateTypeDef = TypedDict(
     "GetServersRequestGetServersPaginateTypeDef",
     {
         "vmServerAddressList": Sequence[VmServerAddressTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetServersRequestRequestTypeDef = TypedDict(
     "GetServersRequestRequestTypeDef",
     {
@@ -718,22 +731,20 @@
     "_OptionalNotifyAppValidationOutputRequestRequestTypeDef",
     {
         "notificationContext": NotificationContextTypeDef,
     },
     total=False,
 )
 
-
 class NotifyAppValidationOutputRequestRequestTypeDef(
     _RequiredNotifyAppValidationOutputRequestRequestTypeDef,
     _OptionalNotifyAppValidationOutputRequestRequestTypeDef,
 ):
     pass
 
-
 ReplicationRunTypeDef = TypedDict(
     "ReplicationRunTypeDef",
     {
         "replicationRunId": str,
         "state": ReplicationRunStateType,
         "type": ReplicationRunTypeType,
         "stageDetails": ReplicationRunStageDetailsTypeDef,
@@ -749,15 +760,15 @@
 )
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppValidationOutputTypeDef = TypedDict(
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
@@ -838,16 +849,26 @@
 GetServersResponseTypeDef = TypedDict(
     "GetServersResponseTypeDef",
     {
         "lastModifiedOn": datetime,
         "serverCatalogStatus": ServerCatalogStatusType,
         "serverList": List[ServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupOutputTypeDef = TypedDict(
+    "ServerGroupOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "name": str,
+        "serverList": List[ServerTypeDef],
     },
+    total=False,
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
         "name": str,
@@ -871,14 +892,23 @@
         "iamInstanceProfileName": str,
         "configureScript": S3LocationTypeDef,
         "configureScriptType": ScriptTypeType,
     },
     total=False,
 )
 
+ServerReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerReplicationConfigurationOutputTypeDef",
+    {
+        "server": ServerTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 ServerReplicationConfigurationTypeDef = TypedDict(
     "ServerReplicationConfigurationTypeDef",
     {
         "server": ServerTypeDef,
         "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
@@ -905,108 +935,111 @@
 )
 
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReplicationRunsResponseTypeDef = TypedDict(
     "GetReplicationRunsResponseTypeDef",
     {
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[ServerGroupTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
+        "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppResponseTypeDef = TypedDict(
     "GetAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
+        "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appId": str,
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "serverGroups": Sequence[ServerGroupTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
+        "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ServerGroupUnionTypeDef = Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]
+ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "launchOrder": int,
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
+    },
+    total=False,
+)
+
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
+        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 ServerGroupReplicationConfigurationTypeDef = TypedDict(
     "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationTypeDef],
+        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupValidationConfigurationTypeDef = TypedDict(
     "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
+        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1017,87 +1050,126 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "clientToken": str,
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
     {
         "appId": str,
+        "name": str,
+        "description": str,
         "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ServerGroupLaunchConfigurationUnionTypeDef = Union[
+    ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
+]
 GetAppReplicationConfigurationResponseTypeDef = TypedDict(
     "GetAppReplicationConfigurationResponseTypeDef",
     {
-        "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "serverGroupReplicationConfigurations": List[
+            ServerGroupReplicationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
+ServerGroupReplicationConfigurationUnionTypeDef = Union[
+    ServerGroupReplicationConfigurationTypeDef, ServerGroupReplicationConfigurationOutputTypeDef
+]
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
     {
-        "appId": str,
-        "serverGroupReplicationConfigurations": Sequence[
-            ServerGroupReplicationConfigurationTypeDef
+        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": List[
+            ServerGroupValidationConfigurationOutputTypeDef
         ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupValidationConfigurationUnionTypeDef = Union[
+    ServerGroupValidationConfigurationTypeDef, ServerGroupValidationConfigurationOutputTypeDef
+]
+GetAppValidationOutputResponseTypeDef = TypedDict(
+    "GetAppValidationOutputResponseTypeDef",
+    {
+        "validationOutputList": List[ValidationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationUnionTypeDef],
     },
     total=False,
 )
 
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
+PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
-        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "serverGroupReplicationConfigurations": Sequence[
+            ServerGroupReplicationConfigurationUnionTypeDef
+        ],
     },
+    total=False,
 )
 
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appValidationConfigurations": Sequence[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": Sequence[ServerGroupValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": Sequence[
+            ServerGroupValidationConfigurationUnionTypeDef
+        ],
     },
     total=False,
 )
 
-
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
-
-
-GetAppValidationOutputResponseTypeDef = TypedDict(
-    "GetAppValidationOutputResponseTypeDef",
-    {
-        "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms/type_defs.pyi` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sms.type_defs import LaunchDetailsTypeDef
 
-    data: LaunchDetailsTypeDef = {...}
+    data: LaunchDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,100 +39,112 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
-    "CreateReplicationJobRequestRequestTypeDef",
-    "CreateReplicationJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
     "S3LocationTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetConnectorsRequestRequestTypeDef",
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationJobsRequestRequestTypeDef",
-    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
-    "ListAppsRequestListAppsPaginateTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
-    "PaginatorConfigTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "ResponseMetadataTypeDef",
-    "ServerReplicationParametersTypeDef",
+    "ServerReplicationParametersOutputTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
-    "StartOnDemandReplicationRunResponseTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
-    "UpdateReplicationJobRequestRequestTypeDef",
     "AppSummaryTypeDef",
+    "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
+    "StartOnDemandReplicationRunResponseTypeDef",
+    "CreateReplicationJobRequestRequestTypeDef",
+    "ServerReplicationParametersTypeDef",
+    "UpdateReplicationJobRequestRequestTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
     "ServerTypeDef",
     "ReplicationJobTypeDef",
     "AppValidationConfigurationTypeDef",
     "GetServersResponseTypeDef",
+    "ServerGroupOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
+    "ServerReplicationConfigurationOutputTypeDef",
     "ServerReplicationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
     "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
-    "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "UpdateAppResponseTypeDef",
+    "ServerGroupUnionTypeDef",
+    "ServerGroupLaunchConfigurationOutputTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
+    "ServerGroupReplicationConfigurationOutputTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
+    "ServerGroupValidationConfigurationOutputTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "ServerGroupLaunchConfigurationUnionTypeDef",
     "GetAppReplicationConfigurationResponseTypeDef",
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "ServerGroupReplicationConfigurationUnionTypeDef",
     "GetAppValidationConfigurationResponseTypeDef",
-    "PutAppValidationConfigurationRequestRequestTypeDef",
+    "ServerGroupValidationConfigurationUnionTypeDef",
     "GetAppValidationOutputResponseTypeDef",
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "PutAppValidationConfigurationRequestRequestTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
         "stackName": str,
@@ -163,50 +175,26 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReplicationJobRequestRequestTypeDef",
-    {
-        "serverId": str,
-        "seedReplicationTime": Union[datetime, str],
-    },
-)
-_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-class CreateReplicationJobRequestRequestTypeDef(
-    _RequiredCreateReplicationJobRequestRequestTypeDef,
-    _OptionalCreateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
-CreateReplicationJobResponseTypeDef = TypedDict(
-    "CreateReplicationJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "replicationJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -311,70 +299,43 @@
 GetAppValidationOutputRequestRequestTypeDef = TypedDict(
     "GetAppValidationOutputRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
-GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetConnectorsRequestRequestTypeDef = TypedDict(
     "GetConnectorsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetReplicationJobsRequestRequestTypeDef = TypedDict(
     "GetReplicationJobsRequestRequestTypeDef",
     {
         "replicationJobId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
-    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetReplicationRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetReplicationRunsRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalGetReplicationRunsRequestRequestTypeDef = TypedDict(
@@ -382,20 +343,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetReplicationRunsRequestRequestTypeDef(
     _RequiredGetReplicationRunsRequestRequestTypeDef,
     _OptionalGetReplicationRunsRequestRequestTypeDef,
 ):
     pass
 
+
 VmServerAddressTypeDef = TypedDict(
     "VmServerAddressTypeDef",
     {
         "vmManagerId": str,
         "vmId": str,
     },
     total=False,
@@ -413,23 +376,14 @@
     "LaunchAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-ListAppsRequestListAppsPaginateTypeDef = TypedDict(
-    "ListAppsRequestListAppsPaginateTypeDef",
-    {
-        "appIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -442,46 +396,25 @@
         "validationId": str,
         "status": ValidationStatusType,
         "statusMessage": str,
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
 ReplicationRunStageDetailsTypeDef = TypedDict(
     "ReplicationRunStageDetailsTypeDef",
     {
         "stage": str,
         "stageProgress": str,
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
-ServerReplicationParametersTypeDef = TypedDict(
-    "ServerReplicationParametersTypeDef",
+ServerReplicationParametersOutputTypeDef = TypedDict(
+    "ServerReplicationParametersOutputTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
@@ -508,47 +441,43 @@
     "_OptionalStartOnDemandAppReplicationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class StartOnDemandAppReplicationRequestRequestTypeDef(
     _RequiredStartOnDemandAppReplicationRequestRequestTypeDef,
     _OptionalStartOnDemandAppReplicationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
-StartOnDemandReplicationRunResponseTypeDef = TypedDict(
-    "StartOnDemandReplicationRunResponseTypeDef",
-    {
-        "replicationRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
@@ -558,41 +487,14 @@
     "TerminateAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "nextReplicationRunStartTime": Union[datetime, str],
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-class UpdateReplicationJobRequestRequestTypeDef(
-    _RequiredUpdateReplicationJobRequestRequestTypeDef,
-    _OptionalUpdateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -611,36 +513,125 @@
         "roleName": str,
         "totalServerGroups": int,
         "totalServers": int,
     },
     total=False,
 )
 
+CreateReplicationJobResponseTypeDef = TypedDict(
+    "CreateReplicationJobResponseTypeDef",
+    {
+        "replicationJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetConnectorsResponseTypeDef = TypedDict(
     "GetConnectorsResponseTypeDef",
     {
         "connectorList": List[ConnectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandReplicationRunResponseTypeDef = TypedDict(
+    "StartOnDemandReplicationRunResponseTypeDef",
+    {
+        "replicationRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationJobRequestRequestTypeDef",
+    {
+        "serverId": str,
+        "seedReplicationTime": TimestampTypeDef,
     },
 )
+_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class CreateReplicationJobRequestRequestTypeDef(
+    _RequiredCreateReplicationJobRequestRequestTypeDef,
+    _OptionalCreateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
+
+ServerReplicationParametersTypeDef = TypedDict(
+    "ServerReplicationParametersTypeDef",
+    {
+        "seedTime": TimestampTypeDef,
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "nextReplicationRunStartTime": TimestampTypeDef,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class UpdateReplicationJobRequestRequestTypeDef(
+    _RequiredUpdateReplicationJobRequestRequestTypeDef,
+    _OptionalUpdateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
         "s3Location": S3LocationTypeDef,
@@ -660,19 +651,67 @@
     "UserDataTypeDef",
     {
         "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
+GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
+    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+):
+    pass
+
+
+ListAppsRequestListAppsPaginateTypeDef = TypedDict(
+    "ListAppsRequestListAppsPaginateTypeDef",
+    {
+        "appIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetServersRequestGetServersPaginateTypeDef = TypedDict(
     "GetServersRequestGetServersPaginateTypeDef",
     {
         "vmServerAddressList": Sequence[VmServerAddressTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetServersRequestRequestTypeDef = TypedDict(
     "GetServersRequestRequestTypeDef",
     {
@@ -705,20 +744,22 @@
     "_OptionalNotifyAppValidationOutputRequestRequestTypeDef",
     {
         "notificationContext": NotificationContextTypeDef,
     },
     total=False,
 )
 
+
 class NotifyAppValidationOutputRequestRequestTypeDef(
     _RequiredNotifyAppValidationOutputRequestRequestTypeDef,
     _OptionalNotifyAppValidationOutputRequestRequestTypeDef,
 ):
     pass
 
+
 ReplicationRunTypeDef = TypedDict(
     "ReplicationRunTypeDef",
     {
         "replicationRunId": str,
         "state": ReplicationRunStateType,
         "type": ReplicationRunTypeType,
         "stageDetails": ReplicationRunStageDetailsTypeDef,
@@ -734,15 +775,15 @@
 )
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppValidationOutputTypeDef = TypedDict(
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
@@ -823,16 +864,26 @@
 GetServersResponseTypeDef = TypedDict(
     "GetServersResponseTypeDef",
     {
         "lastModifiedOn": datetime,
         "serverCatalogStatus": ServerCatalogStatusType,
         "serverList": List[ServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupOutputTypeDef = TypedDict(
+    "ServerGroupOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "name": str,
+        "serverList": List[ServerTypeDef],
     },
+    total=False,
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
         "name": str,
@@ -856,14 +907,23 @@
         "iamInstanceProfileName": str,
         "configureScript": S3LocationTypeDef,
         "configureScriptType": ScriptTypeType,
     },
     total=False,
 )
 
+ServerReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerReplicationConfigurationOutputTypeDef",
+    {
+        "server": ServerTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 ServerReplicationConfigurationTypeDef = TypedDict(
     "ServerReplicationConfigurationTypeDef",
     {
         "server": ServerTypeDef,
         "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
@@ -890,108 +950,111 @@
 )
 
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReplicationRunsResponseTypeDef = TypedDict(
     "GetReplicationRunsResponseTypeDef",
     {
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[ServerGroupTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
+        "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppResponseTypeDef = TypedDict(
     "GetAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
+        "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appId": str,
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "serverGroups": Sequence[ServerGroupTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
+        "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ServerGroupUnionTypeDef = Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]
+ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "launchOrder": int,
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
+    },
+    total=False,
+)
+
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
+        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 ServerGroupReplicationConfigurationTypeDef = TypedDict(
     "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationTypeDef],
+        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupValidationConfigurationTypeDef = TypedDict(
     "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
+        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1002,85 +1065,127 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "clientToken": str,
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
     {
         "appId": str,
+        "name": str,
+        "description": str,
         "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ServerGroupLaunchConfigurationUnionTypeDef = Union[
+    ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
+]
 GetAppReplicationConfigurationResponseTypeDef = TypedDict(
     "GetAppReplicationConfigurationResponseTypeDef",
     {
-        "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "serverGroupReplicationConfigurations": List[
+            ServerGroupReplicationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
+ServerGroupReplicationConfigurationUnionTypeDef = Union[
+    ServerGroupReplicationConfigurationTypeDef, ServerGroupReplicationConfigurationOutputTypeDef
+]
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
     {
-        "appId": str,
-        "serverGroupReplicationConfigurations": Sequence[
-            ServerGroupReplicationConfigurationTypeDef
+        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": List[
+            ServerGroupValidationConfigurationOutputTypeDef
         ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupValidationConfigurationUnionTypeDef = Union[
+    ServerGroupValidationConfigurationTypeDef, ServerGroupValidationConfigurationOutputTypeDef
+]
+GetAppValidationOutputResponseTypeDef = TypedDict(
+    "GetAppValidationOutputResponseTypeDef",
+    {
+        "validationOutputList": List[ValidationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationUnionTypeDef],
     },
     total=False,
 )
 
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
+PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
-        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "serverGroupReplicationConfigurations": Sequence[
+            ServerGroupReplicationConfigurationUnionTypeDef
+        ],
     },
+    total=False,
 )
 
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appValidationConfigurations": Sequence[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": Sequence[ServerGroupValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": Sequence[
+            ServerGroupValidationConfigurationUnionTypeDef
+        ],
     },
     total=False,
 )
 
+
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
-
-GetAppValidationOutputResponseTypeDef = TypedDict(
-    "GetAppValidationOutputResponseTypeDef",
-    {
-        "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/PKG-INFO` & `types-aiobotocore-sms-2.5.2.post1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-sms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sms type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-sms"></a>
 
 # types-aiobotocore-sms
 
 [![PyPI - types-aiobotocore-sms](https://img.shields.io/pypi/v/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sms?color=blue)](https://pypistats.org/packages/types-aiobotocore-sms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms)](https://pepy.tech/project/types-aiobotocore-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -340,112 +307,123 @@
 )
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
-    CreateReplicationJobResponseTypeDef,
+    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
     S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
-    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    ServerReplicationParametersTypeDef,
+    ServerReplicationParametersOutputTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
+    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
+    CreateReplicationJobRequestRequestTypeDef,
+    ServerReplicationParametersTypeDef,
+    UpdateReplicationJobRequestRequestTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
     ServerTypeDef,
     ReplicationJobTypeDef,
     AppValidationConfigurationTypeDef,
     GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
     ServerReplicationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
     ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
-    CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
-    UpdateAppRequestRequestTypeDef,
     UpdateAppResponseTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupLaunchConfigurationOutputTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
+    ServerGroupReplicationConfigurationOutputTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
+    ServerGroupValidationConfigurationOutputTypeDef,
     ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     GetAppValidationOutputResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LaunchDetailsTypeDef:
+def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sms-2.5.2/types_aiobotocore_sms.egg-info/SOURCES.txt` & `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


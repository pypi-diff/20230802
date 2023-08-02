# Comparing `tmp/types-aiobotocore-securitylake-2.5.2.tar.gz` & `tmp/types-aiobotocore-securitylake-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-securitylake-2.5.2.tar", last modified: Sat Jul  8 01:44:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-securitylake-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
```

## Comparing `types-aiobotocore-securitylake-2.5.2.tar` & `types-aiobotocore-securitylake-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.158882 types-aiobotocore-securitylake-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-07-08 01:44:18.154882 types-aiobotocore-securitylake-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:18.158882 types-aiobotocore-securitylake-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.154882 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25766 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-08 01:40:49.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24192 2023-07-08 01:40:49.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-07-08 01:40:49.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:48.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.154882 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-07-08 01:44:17.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:44:18.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:17.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:44:17.000000 types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15531 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.413462 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25772 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25275 2023-08-02 14:49:29.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-securitylake-2.5.2/LICENSE` & `types-aiobotocore-securitylake-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2/PKG-INFO` & `types-aiobotocore-securitylake-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore securitylake type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore securitylake type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-securitylake"></a>
 
 # types-aiobotocore-securitylake
 
 [![PyPI - types-aiobotocore-securitylake](https://img.shields.io/pypi/v/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-securitylake?color=blue)](https://pypistats.org/packages/types-aiobotocore-securitylake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecurityLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
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
@@ -326,80 +325,84 @@
 )
 
 
 def check_value(value: AccessTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_securitylake.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_securitylake.type_defs import (
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
     AwsLogSourceResourceTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
     DataLakeExceptionTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
+    DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
     DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
-    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
     LogSourceTypeDef,
     SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
@@ -411,15 +414,15 @@
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_value() -> AwsIdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-securitylake-2.5.2/README.md` & `types-aiobotocore-securitylake-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-securitylake"></a>
 
 # types-aiobotocore-securitylake
 
 [![PyPI - types-aiobotocore-securitylake](https://img.shields.io/pypi/v/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-securitylake?color=blue)](https://pypistats.org/packages/types-aiobotocore-securitylake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecurityLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
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
@@ -293,80 +293,84 @@
 )
 
 
 def check_value(value: AccessTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_securitylake.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_securitylake.type_defs import (
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
     AwsLogSourceResourceTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
     DataLakeExceptionTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
+    DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
     DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
-    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
     LogSourceTypeDef,
     SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
@@ -378,15 +382,15 @@
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_value() -> AwsIdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-securitylake-2.5.2/setup.py` & `types-aiobotocore-securitylake-2.5.2.post1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-securitylake",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with"
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
-    keywords="aiobotocore securitylake type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore securitylake type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_securitylake": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/"
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/__init__.py` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/__init__.pyi` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/__main__.py` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecurityLake 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SecurityLake 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
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

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/client.py` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     AwsLogSourceConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     CreateDataLakeResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
     DataLakeConfigurationTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
@@ -166,15 +166,17 @@
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_exception_subscription)
         """
 
     async def create_data_lake_organization_configuration(
-        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
+        self,
+        *,
+        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Automatically enables Amazon Security Lake for new member accounts in your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_organization_configuration)
@@ -246,15 +248,17 @@
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake_exception_subscription)
         """
 
     async def delete_data_lake_organization_configuration(
-        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
+        self,
+        *,
+        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Removes automatic the enablement of configuration settings for new member
         accounts (but retains the settings for the delegated administrator) from Amazon
         Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/client.pyi` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     AwsLogSourceConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     CreateDataLakeResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
     DataLakeConfigurationTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
@@ -155,15 +155,17 @@
         Creates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_exception_subscription)
         """
     async def create_data_lake_organization_configuration(
-        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
+        self,
+        *,
+        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Automatically enables Amazon Security Lake for new member accounts in your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_organization_configuration)
@@ -228,15 +230,17 @@
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake_exception_subscription)
         """
     async def delete_data_lake_organization_configuration(
-        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
+        self,
+        *,
+        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Removes automatic the enablement of configuration settings for new member
         accounts (but retains the settings for the delegated administrator) from Amazon
         Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/literals.py` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/literals.pyi` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/paginator.py` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,30 +61,30 @@
 class GetDataLakeSourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#getdatalakesourcespaginator)
     """
 
     def paginate(
-        self, *, accounts: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accounts: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDataLakeSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#getdatalakesourcespaginator)
         """
 
 
 class ListDataLakeExceptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listdatalakeexceptionspaginator)
     """
 
     def paginate(
-        self, *, regions: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, regions: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataLakeExceptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listdatalakeexceptionspaginator)
         """
 
 
@@ -96,28 +96,28 @@
 
     def paginate(
         self,
         *,
         accounts: Sequence[str] = ...,
         regions: Sequence[str] = ...,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listlogsourcespaginator)
         """
 
 
 class ListSubscribersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listsubscriberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSubscribersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listsubscriberspaginator)
         """
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/paginator.pyi` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 class GetDataLakeSourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#getdatalakesourcespaginator)
     """
 
     def paginate(
-        self, *, accounts: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accounts: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDataLakeSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#getdatalakesourcespaginator)
         """
 
 class ListDataLakeExceptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listdatalakeexceptionspaginator)
     """
 
     def paginate(
-        self, *, regions: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, regions: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataLakeExceptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listdatalakeexceptionspaginator)
         """
 
 class ListLogSourcesPaginator(AioPaginator):
@@ -91,27 +91,27 @@
 
     def paginate(
         self,
         *,
         accounts: Sequence[str] = ...,
         regions: Sequence[str] = ...,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listlogsourcespaginator)
         """
 
 class ListSubscribersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listsubscriberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSubscribersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listsubscriberspaginator)
         """
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/type_defs.py` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_securitylake.type_defs import AwsIdentityTypeDef
 
-    data: AwsIdentityTypeDef = {...}
+    data: AwsIdentityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessTypeType,
     AwsLogSourceNameType,
     DataLakeStatusType,
     HttpMethodType,
     SourceCollectionStatusType,
@@ -25,73 +25,76 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
     "AwsLogSourceResourceTypeDef",
-    "CreateAwsLogSourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "CreateSubscriberNotificationResponseTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
     "DataLakeExceptionTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
+    "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
-    "DeleteAwsLogSourceResponseTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
     "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "ListSubscribersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "UpdateSubscriberNotificationResponseTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    "CreateAwsLogSourceResponseTypeDef",
+    "CreateSubscriberNotificationResponseTypeDef",
+    "DeleteAwsLogSourceResponseTypeDef",
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    "UpdateSubscriberNotificationResponseTypeDef",
     "CustomLogSourceConfigurationTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
+    "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationUnionTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
     "LogSourceTypeDef",
     "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
@@ -126,35 +129,36 @@
     {
         "accounts": Sequence[str],
         "sourceVersion": str,
     },
     total=False,
 )
 
-
 class AwsLogSourceConfigurationTypeDef(
     _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
 ):
     pass
 
-
 AwsLogSourceResourceTypeDef = TypedDict(
     "AwsLogSourceResourceTypeDef",
     {
         "sourceName": AwsLogSourceNameType,
         "sourceVersion": str,
     },
     total=False,
 )
 
-CreateAwsLogSourceResponseTypeDef = TypedDict(
-    "CreateAwsLogSourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
@@ -165,30 +169,20 @@
     "_OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "exceptionTimeToLive": int,
     },
     total=False,
 )
 
-
 class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
-CreateSubscriberNotificationResponseTypeDef = TypedDict(
-    "CreateSubscriberNotificationResponseTypeDef",
-    {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
         "databaseArn": str,
         "tableArn": str,
     },
@@ -252,14 +246,23 @@
     {
         "days": int,
         "storageClass": str,
     },
     total=False,
 )
 
+DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
+    "DataLakeReplicationConfigurationOutputTypeDef",
+    {
+        "regions": List[str],
+        "roleArn": str,
+    },
+    total=False,
+)
+
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
     total=False,
@@ -270,44 +273,34 @@
     {
         "code": str,
         "reason": str,
     },
     total=False,
 )
 
-DeleteAwsLogSourceResponseTypeDef = TypedDict(
-    "DeleteAwsLogSourceResponseTypeDef",
-    {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceVersion": str,
     },
     total=False,
 )
 
-
 class DeleteCustomLogSourceRequestRequestTypeDef(
     _RequiredDeleteCustomLogSourceRequestRequestTypeDef,
     _OptionalDeleteCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteDataLakeRequestRequestTypeDef = TypedDict(
     "DeleteDataLakeRequestRequestTypeDef",
     {
         "regions": Sequence[str],
     },
 )
 
@@ -321,29 +314,20 @@
 DeleteSubscriberRequestRequestTypeDef = TypedDict(
     "DeleteSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 
-GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    {
-        "exceptionTimeToLive": int,
-        "notificationEndpoint": str,
-        "subscriptionProtocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "accounts": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetDataLakeSourcesRequestRequestTypeDef = TypedDict(
     "GetDataLakeSourcesRequestRequestTypeDef",
     {
@@ -374,30 +358,19 @@
         "authorizationApiKeyName": str,
         "authorizationApiKeyValue": str,
         "httpMethod": HttpMethodType,
     },
     total=False,
 )
 
-
 class HttpsNotificationConfigurationTypeDef(
     _RequiredHttpsNotificationConfigurationTypeDef, _OptionalHttpsNotificationConfigurationTypeDef
 ):
     pass
 
-
-ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
-    {
-        "regions": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataLakeExceptionsRequestRequestTypeDef = TypedDict(
     "ListDataLakeExceptionsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "regions": Sequence[str],
     },
@@ -408,59 +381,30 @@
     "ListDataLakesRequestRequestTypeDef",
     {
         "regions": Sequence[str],
     },
     total=False,
 )
 
-ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribersRequestRequestTypeDef = TypedDict(
     "ListSubscribersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
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
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
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
 _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
         "subscriptionProtocol": str,
     },
 )
@@ -468,52 +412,92 @@
     "_OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "exceptionTimeToLive": int,
     },
     total=False,
 )
 
-
 class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateSubscriberNotificationResponseTypeDef = TypedDict(
-    "UpdateSubscriberNotificationResponseTypeDef",
-    {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAwsLogSourceRequestRequestTypeDef = TypedDict(
     "CreateAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
 DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
     "DeleteAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
+DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
+    {
+        "region": str,
+        "sources": List[AwsLogSourceResourceTypeDef],
+    },
+)
+
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
         "sources": Sequence[AwsLogSourceResourceTypeDef],
     },
 )
 
+CreateAwsLogSourceResponseTypeDef = TypedDict(
+    "CreateAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriberNotificationResponseTypeDef = TypedDict(
+    "CreateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAwsLogSourceResponseTypeDef = TypedDict(
+    "DeleteAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    {
+        "exceptionTimeToLive": int,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSubscriberNotificationResponseTypeDef = TypedDict(
+    "UpdateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CustomLogSourceConfigurationTypeDef = TypedDict(
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
@@ -530,18 +514,27 @@
 )
 
 ListDataLakeExceptionsResponseTypeDef = TypedDict(
     "ListDataLakeExceptionsResponseTypeDef",
     {
         "exceptions": List[DataLakeExceptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleConfigurationOutputTypeDef",
+    {
+        "expiration": DataLakeLifecycleExpirationTypeDef,
+        "transitions": List[DataLakeLifecycleTransitionTypeDef],
+    },
+    total=False,
+)
+
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
         "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
     },
     total=False,
@@ -564,45 +557,61 @@
         "exception": DataLakeUpdateExceptionTypeDef,
         "requestId": str,
         "status": DataLakeStatusType,
     },
     total=False,
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
+GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     {
-        "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
-        "sqsNotificationConfiguration": Mapping[str, Any],
+        "accounts": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+        "regions": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
     {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+        "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
+        "sqsNotificationConfiguration": Mapping[str, Any],
     },
+    total=False,
 )
 
 GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeAutoEnableNewAccountConfigurationUnionTypeDef = Union[
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
+]
 _RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
@@ -611,27 +620,25 @@
         "configuration": CustomLogSourceConfigurationTypeDef,
         "eventClasses": Sequence[str],
         "sourceVersion": str,
     },
     total=False,
 )
 
-
 class CreateCustomLogSourceRequestRequestTypeDef(
     _RequiredCreateCustomLogSourceRequestRequestTypeDef,
     _OptionalCreateCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
-
 CreateCustomLogSourceResponseTypeDef = TypedDict(
     "CreateCustomLogSourceResponseTypeDef",
     {
         "source": CustomLogSourceResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LogSourceResourceTypeDef = TypedDict(
     "LogSourceResourceTypeDef",
     {
         "awsLogSource": AwsLogSourceResourceTypeDef,
@@ -652,28 +659,26 @@
         "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
         "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
         "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DataLakeConfigurationTypeDef(
     _RequiredDataLakeConfigurationTypeDef, _OptionalDataLakeConfigurationTypeDef
 ):
     pass
 
-
 GetDataLakeSourcesResponseTypeDef = TypedDict(
     "GetDataLakeSourcesResponseTypeDef",
     {
         "dataLakeArn": str,
         "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataLakeResourceTypeDef = TypedDict(
     "_RequiredDataLakeResourceTypeDef",
     {
         "dataLakeArn": str,
@@ -681,27 +686,25 @@
     },
 )
 _OptionalDataLakeResourceTypeDef = TypedDict(
     "_OptionalDataLakeResourceTypeDef",
     {
         "createStatus": DataLakeStatusType,
         "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
-        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
-        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
     total=False,
 )
 
-
 class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
     pass
 
-
 CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
     "CreateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
@@ -710,14 +713,28 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
+CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
+    },
+)
+
+DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
+    },
+)
+
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
@@ -727,28 +744,26 @@
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
     },
     total=False,
 )
 
-
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
 ):
     pass
 
-
 ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     {
         "accounts": Sequence[str],
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListLogSourcesRequestRequestTypeDef = TypedDict(
     "ListLogSourcesRequestRequestTypeDef",
     {
@@ -794,21 +809,19 @@
         "subscriberEndpoint": str,
         "subscriberStatus": SubscriberStatusType,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-
 class SubscriberResourceTypeDef(
     _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
 ):
     pass
 
-
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
@@ -818,21 +831,19 @@
         "subscriberDescription": str,
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
     total=False,
 )
 
-
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
-
 CreateDataLakeRequestRequestTypeDef = TypedDict(
     "CreateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
         "metaStoreManagerRoleArn": str,
     },
 )
@@ -844,68 +855,68 @@
     },
 )
 
 CreateDataLakeResponseTypeDef = TypedDict(
     "CreateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataLakesResponseTypeDef = TypedDict(
     "ListDataLakesResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataLakeResponseTypeDef = TypedDict(
     "UpdateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSourcesResponseTypeDef = TypedDict(
     "ListLogSourcesResponseTypeDef",
     {
         "nextToken": str,
         "sources": List[LogSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubscriberResponseTypeDef = TypedDict(
     "CreateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSubscriberResponseTypeDef = TypedDict(
     "GetSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribersResponseTypeDef = TypedDict(
     "ListSubscribersResponseTypeDef",
     {
         "nextToken": str,
         "subscribers": List[SubscriberResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSubscriberResponseTypeDef = TypedDict(
     "UpdateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake/type_defs.pyi` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_securitylake.type_defs import AwsIdentityTypeDef
 
-    data: AwsIdentityTypeDef = {...}
+    data: AwsIdentityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessTypeType,
     AwsLogSourceNameType,
     DataLakeStatusType,
     HttpMethodType,
     SourceCollectionStatusType,
@@ -25,72 +25,77 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
     "AwsLogSourceResourceTypeDef",
-    "CreateAwsLogSourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "CreateSubscriberNotificationResponseTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
     "DataLakeExceptionTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
+    "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
-    "DeleteAwsLogSourceResponseTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
     "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "ListSubscribersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "UpdateSubscriberNotificationResponseTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    "CreateAwsLogSourceResponseTypeDef",
+    "CreateSubscriberNotificationResponseTypeDef",
+    "DeleteAwsLogSourceResponseTypeDef",
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    "UpdateSubscriberNotificationResponseTypeDef",
     "CustomLogSourceConfigurationTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
+    "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationUnionTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
     "LogSourceTypeDef",
     "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
@@ -125,33 +130,38 @@
     {
         "accounts": Sequence[str],
         "sourceVersion": str,
     },
     total=False,
 )
 
+
 class AwsLogSourceConfigurationTypeDef(
     _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
 ):
     pass
 
+
 AwsLogSourceResourceTypeDef = TypedDict(
     "AwsLogSourceResourceTypeDef",
     {
         "sourceName": AwsLogSourceNameType,
         "sourceVersion": str,
     },
     total=False,
 )
 
-CreateAwsLogSourceResponseTypeDef = TypedDict(
-    "CreateAwsLogSourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
@@ -162,27 +172,21 @@
     "_OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "exceptionTimeToLive": int,
     },
     total=False,
 )
 
+
 class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-CreateSubscriberNotificationResponseTypeDef = TypedDict(
-    "CreateSubscriberNotificationResponseTypeDef",
-    {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
         "databaseArn": str,
         "tableArn": str,
@@ -247,14 +251,23 @@
     {
         "days": int,
         "storageClass": str,
     },
     total=False,
 )
 
+DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
+    "DataLakeReplicationConfigurationOutputTypeDef",
+    {
+        "regions": List[str],
+        "roleArn": str,
+    },
+    total=False,
+)
+
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
     total=False,
@@ -265,42 +278,36 @@
     {
         "code": str,
         "reason": str,
     },
     total=False,
 )
 
-DeleteAwsLogSourceResponseTypeDef = TypedDict(
-    "DeleteAwsLogSourceResponseTypeDef",
-    {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceVersion": str,
     },
     total=False,
 )
 
+
 class DeleteCustomLogSourceRequestRequestTypeDef(
     _RequiredDeleteCustomLogSourceRequestRequestTypeDef,
     _OptionalDeleteCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteDataLakeRequestRequestTypeDef = TypedDict(
     "DeleteDataLakeRequestRequestTypeDef",
     {
         "regions": Sequence[str],
     },
 )
 
@@ -314,29 +321,20 @@
 DeleteSubscriberRequestRequestTypeDef = TypedDict(
     "DeleteSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 
-GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    {
-        "exceptionTimeToLive": int,
-        "notificationEndpoint": str,
-        "subscriptionProtocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "accounts": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetDataLakeSourcesRequestRequestTypeDef = TypedDict(
     "GetDataLakeSourcesRequestRequestTypeDef",
     {
@@ -367,27 +365,20 @@
         "authorizationApiKeyName": str,
         "authorizationApiKeyValue": str,
         "httpMethod": HttpMethodType,
     },
     total=False,
 )
 
+
 class HttpsNotificationConfigurationTypeDef(
     _RequiredHttpsNotificationConfigurationTypeDef, _OptionalHttpsNotificationConfigurationTypeDef
 ):
     pass
 
-ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
-    {
-        "regions": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDataLakeExceptionsRequestRequestTypeDef = TypedDict(
     "ListDataLakeExceptionsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "regions": Sequence[str],
@@ -399,59 +390,30 @@
     "ListDataLakesRequestRequestTypeDef",
     {
         "regions": Sequence[str],
     },
     total=False,
 )
 
-ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribersRequestRequestTypeDef = TypedDict(
     "ListSubscribersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
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
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
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
 _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
         "subscriptionProtocol": str,
     },
 )
@@ -459,27 +421,21 @@
     "_OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "exceptionTimeToLive": int,
     },
     total=False,
 )
 
+
 class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-UpdateSubscriberNotificationResponseTypeDef = TypedDict(
-    "UpdateSubscriberNotificationResponseTypeDef",
-    {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateAwsLogSourceRequestRequestTypeDef = TypedDict(
     "CreateAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
@@ -487,22 +443,72 @@
 DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
     "DeleteAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
+DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
+    {
+        "region": str,
+        "sources": List[AwsLogSourceResourceTypeDef],
+    },
+)
+
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
         "sources": Sequence[AwsLogSourceResourceTypeDef],
     },
 )
 
+CreateAwsLogSourceResponseTypeDef = TypedDict(
+    "CreateAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriberNotificationResponseTypeDef = TypedDict(
+    "CreateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAwsLogSourceResponseTypeDef = TypedDict(
+    "DeleteAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    {
+        "exceptionTimeToLive": int,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSubscriberNotificationResponseTypeDef = TypedDict(
+    "UpdateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CustomLogSourceConfigurationTypeDef = TypedDict(
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
@@ -519,16 +525,25 @@
 )
 
 ListDataLakeExceptionsResponseTypeDef = TypedDict(
     "ListDataLakeExceptionsResponseTypeDef",
     {
         "exceptions": List[DataLakeExceptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleConfigurationOutputTypeDef",
+    {
+        "expiration": DataLakeLifecycleExpirationTypeDef,
+        "transitions": List[DataLakeLifecycleTransitionTypeDef],
     },
+    total=False,
 )
 
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
         "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
@@ -553,45 +568,61 @@
         "exception": DataLakeUpdateExceptionTypeDef,
         "requestId": str,
         "status": DataLakeStatusType,
     },
     total=False,
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
+GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     {
-        "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
-        "sqsNotificationConfiguration": Mapping[str, Any],
+        "accounts": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+        "regions": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
+        "sqsNotificationConfiguration": Mapping[str, Any],
+    },
+    total=False,
 )
 
 GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeAutoEnableNewAccountConfigurationUnionTypeDef = Union[
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
+]
 _RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
@@ -600,25 +631,27 @@
         "configuration": CustomLogSourceConfigurationTypeDef,
         "eventClasses": Sequence[str],
         "sourceVersion": str,
     },
     total=False,
 )
 
+
 class CreateCustomLogSourceRequestRequestTypeDef(
     _RequiredCreateCustomLogSourceRequestRequestTypeDef,
     _OptionalCreateCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
+
 CreateCustomLogSourceResponseTypeDef = TypedDict(
     "CreateCustomLogSourceResponseTypeDef",
     {
         "source": CustomLogSourceResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LogSourceResourceTypeDef = TypedDict(
     "LogSourceResourceTypeDef",
     {
         "awsLogSource": AwsLogSourceResourceTypeDef,
@@ -639,26 +672,28 @@
         "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
         "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
         "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DataLakeConfigurationTypeDef(
     _RequiredDataLakeConfigurationTypeDef, _OptionalDataLakeConfigurationTypeDef
 ):
     pass
 
+
 GetDataLakeSourcesResponseTypeDef = TypedDict(
     "GetDataLakeSourcesResponseTypeDef",
     {
         "dataLakeArn": str,
         "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataLakeResourceTypeDef = TypedDict(
     "_RequiredDataLakeResourceTypeDef",
     {
         "dataLakeArn": str,
@@ -666,25 +701,27 @@
     },
 )
 _OptionalDataLakeResourceTypeDef = TypedDict(
     "_OptionalDataLakeResourceTypeDef",
     {
         "createStatus": DataLakeStatusType,
         "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
-        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
-        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
     total=False,
 )
 
+
 class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
     pass
 
+
 CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
     "CreateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
@@ -693,14 +730,28 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
+CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
+    },
+)
+
+DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
+    },
+)
+
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
@@ -710,26 +761,28 @@
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
     },
     total=False,
 )
 
+
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
 ):
     pass
 
+
 ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     {
         "accounts": Sequence[str],
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListLogSourcesRequestRequestTypeDef = TypedDict(
     "ListLogSourcesRequestRequestTypeDef",
     {
@@ -775,19 +828,21 @@
         "subscriberEndpoint": str,
         "subscriberStatus": SubscriberStatusType,
         "updatedAt": datetime,
     },
     total=False,
 )
 
+
 class SubscriberResourceTypeDef(
     _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
 ):
     pass
 
+
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
@@ -797,19 +852,21 @@
         "subscriberDescription": str,
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
     total=False,
 )
 
+
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
+
 CreateDataLakeRequestRequestTypeDef = TypedDict(
     "CreateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
         "metaStoreManagerRoleArn": str,
     },
 )
@@ -821,68 +878,68 @@
     },
 )
 
 CreateDataLakeResponseTypeDef = TypedDict(
     "CreateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataLakesResponseTypeDef = TypedDict(
     "ListDataLakesResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataLakeResponseTypeDef = TypedDict(
     "UpdateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSourcesResponseTypeDef = TypedDict(
     "ListLogSourcesResponseTypeDef",
     {
         "nextToken": str,
         "sources": List[LogSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubscriberResponseTypeDef = TypedDict(
     "CreateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSubscriberResponseTypeDef = TypedDict(
     "GetSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribersResponseTypeDef = TypedDict(
     "ListSubscribersResponseTypeDef",
     {
         "nextToken": str,
         "subscribers": List[SubscriberResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSubscriberResponseTypeDef = TypedDict(
     "UpdateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/PKG-INFO` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore securitylake type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore securitylake type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-securitylake"></a>
 
 # types-aiobotocore-securitylake
 
 [![PyPI - types-aiobotocore-securitylake](https://img.shields.io/pypi/v/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-securitylake?color=blue)](https://pypistats.org/packages/types-aiobotocore-securitylake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecurityLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
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
@@ -326,80 +325,84 @@
 )
 
 
 def check_value(value: AccessTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_securitylake.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_securitylake.type_defs import (
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
     AwsLogSourceResourceTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
     DataLakeExceptionTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
+    DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
     DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
-    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
     LogSourceTypeDef,
     SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
@@ -411,15 +414,15 @@
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_value() -> AwsIdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-securitylake-2.5.2/types_aiobotocore_securitylake.egg-info/SOURCES.txt` & `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*


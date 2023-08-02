# Comparing `tmp/types-aiobotocore-finspace-2.5.2.tar.gz` & `tmp/types-aiobotocore-finspace-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-2.5.2.tar", last modified: Sat Jul  8 01:43:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:18 2023, max compression
```

## Comparing `types-aiobotocore-finspace-2.5.2.tar` & `types-aiobotocore-finspace-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.638132 types-aiobotocore-finspace-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-08 01:43:37.638132 types-aiobotocore-finspace-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:37.638132 types-aiobotocore-finspace-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:30:50.000000 types-aiobotocore-finspace-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.638132 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34947 2023-07-08 01:30:52.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34909 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:51.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.638132 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-08 01:43:37.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:43:37.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:37.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:37.000000 types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26537 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36840 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-2.5.2/LICENSE` & `types-aiobotocore-finspace-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2/PKG-INFO` & `types-aiobotocore-finspace-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore finspace type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore finspace type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-finspace"></a>
 
 # types-aiobotocore-finspace
 
 [![PyPI - types-aiobotocore-finspace](https://img.shields.io/pypi/v/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-finspace?color=blue)](https://pypistats.org/packages/types-aiobotocore-finspace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.finspace 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [types-aiobotocore-finspace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/).
 
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
@@ -319,112 +318,119 @@
 )
 
 
 def check_value(value: AutoScalingMetricType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_finspace.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    CreateEnvironmentResponseTypeDef,
+    ResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
+    VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
-    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
-    CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
+    FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
-    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
-    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
     TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
-    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
+    KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    CreateKxDatabaseResponseTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
+    CreateKxUserResponseTypeDef,
+    GetKxConnectionStringResponseTypeDef,
+    GetKxDatabaseResponseTypeDef,
+    GetKxUserResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    VpcConfigurationUnionTypeDef,
+    EnvironmentTypeDef,
+    FederationParametersUnionTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
-    CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
+    CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_value() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-finspace-2.5.2/README.md` & `types-aiobotocore-finspace-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-finspace"></a>
 
 # types-aiobotocore-finspace
 
 [![PyPI - types-aiobotocore-finspace](https://img.shields.io/pypi/v/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-finspace?color=blue)](https://pypistats.org/packages/types-aiobotocore-finspace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.finspace 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [types-aiobotocore-finspace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/).
 
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
@@ -286,112 +286,119 @@
 )
 
 
 def check_value(value: AutoScalingMetricType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_finspace.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    CreateEnvironmentResponseTypeDef,
+    ResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
+    VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
-    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
-    CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
+    FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
-    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
-    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
     TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
-    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
+    KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    CreateKxDatabaseResponseTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
+    CreateKxUserResponseTypeDef,
+    GetKxConnectionStringResponseTypeDef,
+    GetKxDatabaseResponseTypeDef,
+    GetKxUserResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    VpcConfigurationUnionTypeDef,
+    EnvironmentTypeDef,
+    FederationParametersUnionTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
-    CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
+    CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_value() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-finspace-2.5.2/setup.py` & `types-aiobotocore-finspace-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore finspace type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore finspace type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_finspace": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/"
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/__init__.py` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/__init__.pyi` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/__main__.py` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.finspace 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.finspace 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/client.py` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
-    FederationParametersTypeDef,
+    FederationParametersUnionTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
-    KxDatabaseConfigurationTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
@@ -57,15 +57,15 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -132,15 +132,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...,
+        federationParameters: FederationParametersUnionTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
@@ -168,19 +168,19 @@
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
@@ -466,29 +466,29 @@
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...
+        federationParameters: FederationParametersUnionTypeDef = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_environment)
         """
 
     async def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[KxDatabaseConfigurationTypeDef],
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/client.pyi` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
-    FederationParametersTypeDef,
+    FederationParametersUnionTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
-    KxDatabaseConfigurationTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
@@ -57,15 +57,15 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -125,15 +125,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...,
+        federationParameters: FederationParametersUnionTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
@@ -159,19 +159,19 @@
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
@@ -430,28 +430,28 @@
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...
+        federationParameters: FederationParametersUnionTypeDef = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_environment)
         """
     async def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[KxDatabaseConfigurationTypeDef],
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/literals.py` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/literals.pyi` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/paginator.py` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListKxEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/paginators/#listkxenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKxEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/paginators/#listkxenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/paginator.pyi` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListKxEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/paginators/#listkxenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKxEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/paginators/#listkxenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/type_defs.py` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_finspace.type_defs import AutoScalingConfigurationTypeDef
 
-    data: AutoScalingConfigurationTypeDef = {...}
+    data: AutoScalingConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ChangesetStatusType,
     ChangeTypeType,
     EnvironmentStatusType,
     ErrorDetailsType,
     FederationModeType,
@@ -41,92 +41,99 @@
 __all__ = (
     "AutoScalingConfigurationTypeDef",
     "CapacityConfigurationTypeDef",
     "ChangeRequestTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
-    "CreateEnvironmentResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
-    "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
-    "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
-    "CreateKxUserResponseTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
+    "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
-    "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
-    "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
     "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
-    "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
+    "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
     "ListKxClustersRequestRequestTypeDef",
     "ListKxDatabasesRequestRequestTypeDef",
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
-    "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
-    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
-    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "CreateKxDatabaseResponseTypeDef",
+    "CreateKxEnvironmentResponseTypeDef",
+    "CreateKxUserResponseTypeDef",
+    "GetKxConnectionStringResponseTypeDef",
+    "GetKxDatabaseResponseTypeDef",
+    "GetKxUserResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateKxDatabaseResponseTypeDef",
+    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
+    "VpcConfigurationUnionTypeDef",
+    "EnvironmentTypeDef",
+    "FederationParametersUnionTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
+    "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
-    "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
+    "KxDatabaseConfigurationUnionTypeDef",
+    "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
@@ -196,21 +203,22 @@
     {
         "emailAddress": str,
         "firstName": str,
         "lastName": str,
     },
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "environmentArn": str,
-        "environmentUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "errorMessage": str,
@@ -251,14 +259,25 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "vpcId": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "ipAddressType": Literal["IP_V4"],
+    },
+    total=False,
+)
+
 _RequiredCreateKxDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -275,27 +294,14 @@
 
 class CreateKxDatabaseRequestRequestTypeDef(
     _RequiredCreateKxDatabaseRequestRequestTypeDef, _OptionalCreateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
 
-CreateKxDatabaseResponseTypeDef = TypedDict(
-    "CreateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxEnvironmentRequestRequestTypeDef",
     {
         "name": str,
         "kmsKeyId": str,
     },
 )
@@ -313,28 +319,14 @@
 class CreateKxEnvironmentRequestRequestTypeDef(
     _RequiredCreateKxEnvironmentRequestRequestTypeDef,
     _OptionalCreateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
 
-CreateKxEnvironmentResponseTypeDef = TypedDict(
-    "CreateKxEnvironmentResponseTypeDef",
-    {
-        "name": str,
-        "status": EnvironmentStatusType,
-        "environmentId": str,
-        "description": str,
-        "environmentArn": str,
-        "kmsKeyId": str,
-        "creationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -351,25 +343,14 @@
 
 class CreateKxUserRequestRequestTypeDef(
     _RequiredCreateKxUserRequestRequestTypeDef, _OptionalCreateKxUserRequestRequestTypeDef
 ):
     pass
 
 
-CreateKxUserResponseTypeDef = TypedDict(
-    "CreateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -423,14 +404,27 @@
     "DeleteKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
+FederationParametersOutputTypeDef = TypedDict(
+    "FederationParametersOutputTypeDef",
+    {
+        "samlMetadataDocument": str,
+        "samlMetadataURL": str,
+        "applicationCallBackURL": str,
+        "federationURN": str,
+        "federationProviderName": str,
+        "attributeMap": Dict[str, str],
+    },
+    total=False,
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -456,47 +450,22 @@
     {
         "userArn": str,
         "environmentId": str,
         "clusterName": str,
     },
 )
 
-GetKxConnectionStringResponseTypeDef = TypedDict(
-    "GetKxConnectionStringResponseTypeDef",
-    {
-        "signedConnectionString": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxDatabaseRequestRequestTypeDef = TypedDict(
     "GetKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
     },
 )
 
-GetKxDatabaseResponseTypeDef = TypedDict(
-    "GetKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "lastCompletedChangesetId": str,
-        "numBytes": int,
-        "numChangesets": int,
-        "numFiles": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -512,25 +481,14 @@
     "GetKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
-GetKxUserResponseTypeDef = TypedDict(
-    "GetKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KxChangesetListEntryTypeDef = TypedDict(
     "KxChangesetListEntryTypeDef",
     {
         "changesetId": str,
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
@@ -554,14 +512,22 @@
         "availabilityZoneId": str,
         "lastModifiedTimestamp": datetime,
         "createdTimestamp": datetime,
     },
     total=False,
 )
 
+KxDatabaseCacheConfigurationOutputTypeDef = TypedDict(
+    "KxDatabaseCacheConfigurationOutputTypeDef",
+    {
+        "cacheType": str,
+        "dbPaths": List[str],
+    },
+)
+
 KxDatabaseCacheConfigurationTypeDef = TypedDict(
     "KxDatabaseCacheConfigurationTypeDef",
     {
         "cacheType": str,
         "dbPaths": Sequence[str],
     },
 )
@@ -695,18 +661,20 @@
 
 class ListKxDatabasesRequestRequestTypeDef(
     _RequiredListKxDatabasesRequestRequestTypeDef, _OptionalListKxDatabasesRequestRequestTypeDef
 ):
     pass
 
 
-ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
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
 
 ListKxEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListKxEnvironmentsRequestRequestTypeDef",
     {
@@ -741,43 +709,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -809,25 +748,14 @@
 
 class UpdateKxDatabaseRequestRequestTypeDef(
     _RequiredUpdateKxDatabaseRequestRequestTypeDef, _OptionalUpdateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
 
-UpdateKxDatabaseResponseTypeDef = TypedDict(
-    "UpdateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "environmentId": str,
-        "description": str,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
@@ -867,54 +795,24 @@
 
 class UpdateKxUserRequestRequestTypeDef(
     _RequiredUpdateKxUserRequestRequestTypeDef, _OptionalUpdateKxUserRequestRequestTypeDef
 ):
     pass
 
 
-UpdateKxUserResponseTypeDef = TypedDict(
-    "UpdateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKxChangesetRequestRequestTypeDef = TypedDict(
     "CreateKxChangesetRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
     },
 )
 
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "name": str,
-        "environmentId": str,
-        "awsAccountId": str,
-        "status": EnvironmentStatusType,
-        "environmentUrl": str,
-        "description": str,
-        "environmentArn": str,
-        "sageMakerStudioDomainUrl": str,
-        "kmsKeyId": str,
-        "dedicatedServiceAccountId": str,
-        "federationMode": FederationModeType,
-        "federationParameters": FederationParametersTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -958,26 +856,140 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "environmentArn": str,
+        "environmentUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxDatabaseResponseTypeDef = TypedDict(
+    "CreateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxEnvironmentResponseTypeDef = TypedDict(
+    "CreateKxEnvironmentResponseTypeDef",
+    {
+        "name": str,
+        "status": EnvironmentStatusType,
+        "environmentId": str,
+        "description": str,
+        "environmentArn": str,
+        "kmsKeyId": str,
+        "creationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxUserResponseTypeDef = TypedDict(
+    "CreateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxConnectionStringResponseTypeDef = TypedDict(
+    "GetKxConnectionStringResponseTypeDef",
+    {
+        "signedConnectionString": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxDatabaseResponseTypeDef = TypedDict(
+    "GetKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "lastCompletedChangesetId": str,
+        "numBytes": int,
+        "numChangesets": int,
+        "numFiles": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxUserResponseTypeDef = TypedDict(
+    "GetKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
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
+UpdateKxDatabaseResponseTypeDef = TypedDict(
+    "UpdateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "environmentId": str,
+        "description": str,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKxUserResponseTypeDef = TypedDict(
+    "UpdateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
@@ -985,18 +997,41 @@
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "name": str,
+        "environmentId": str,
+        "awsAccountId": str,
+        "status": EnvironmentStatusType,
+        "environmentUrl": str,
+        "description": str,
+        "environmentArn": str,
+        "sageMakerStudioDomainUrl": str,
+        "kmsKeyId": str,
+        "dedicatedServiceAccountId": str,
+        "federationMode": FederationModeType,
+        "federationParameters": FederationParametersOutputTypeDef,
     },
+    total=False,
 )
 
+FederationParametersUnionTypeDef = Union[
+    FederationParametersTypeDef, FederationParametersOutputTypeDef
+]
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1009,15 +1044,15 @@
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KxEnvironmentTypeDef = TypedDict(
     "KxEnvironmentTypeDef",
     {
         "name": str,
@@ -1080,15 +1115,15 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKxEnvironmentResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1103,36 +1138,58 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxChangesetsResponseTypeDef = TypedDict(
     "ListKxChangesetsResponseTypeDef",
     {
         "kxChangesets": List[KxChangesetListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClustersResponseTypeDef = TypedDict(
     "ListKxClustersResponseTypeDef",
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKxDatabaseConfigurationOutputTypeDef",
+    {
+        "databaseName": str,
+    },
+)
+_OptionalKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKxDatabaseConfigurationOutputTypeDef",
+    {
+        "cacheConfigurations": List[KxDatabaseCacheConfigurationOutputTypeDef],
+        "changesetId": str,
+    },
+    total=False,
+)
+
+
+class KxDatabaseConfigurationOutputTypeDef(
+    _RequiredKxDatabaseConfigurationOutputTypeDef, _OptionalKxDatabaseConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
     },
 )
 _OptionalKxDatabaseConfigurationTypeDef = TypedDict(
@@ -1152,169 +1209,180 @@
 
 
 ListKxDatabasesResponseTypeDef = TypedDict(
     "ListKxDatabasesResponseTypeDef",
     {
         "kxDatabases": List[KxDatabaseListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClusterNodesResponseTypeDef = TypedDict(
     "ListKxClusterNodesResponseTypeDef",
     {
         "nodes": List[KxNodeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxUsersResponseTypeDef = TypedDict(
     "ListKxUsersResponseTypeDef",
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxEnvironmentsResponseTypeDef = TypedDict(
     "ListKxEnvironmentsResponseTypeDef",
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKxClusterRequestRequestTypeDef",
+CreateKxClusterResponseTypeDef = TypedDict(
+    "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
+        "status": KxClusterStatusType,
+        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
-        "releaseLabel": str,
-        "azMode": KxAzModeType,
-    },
-)
-_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKxClusterRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
+        "releaseLabel": str,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
+        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "tags": Mapping[str, str],
+        "createdTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateKxClusterRequestRequestTypeDef(
-    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
-):
-    pass
-
-
-CreateKxClusterResponseTypeDef = TypedDict(
-    "CreateKxClusterResponseTypeDef",
+GetKxClusterResponseTypeDef = TypedDict(
+    "GetKxClusterResponseTypeDef",
     {
-        "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
         "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
         "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetKxClusterResponseTypeDef = TypedDict(
-    "GetKxClusterResponseTypeDef",
+KxDatabaseConfigurationUnionTypeDef = Union[
+    KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef
+]
+_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
-        "status": KxClusterStatusType,
-        "statusReason": str,
+        "environmentId": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
+        "azMode": KxAzModeType,
+    },
+)
+_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKxClusterRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
+        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
-        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
-        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+
+class CreateKxClusterRequestRequestTypeDef(
+    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace/type_defs.pyi` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_finspace.type_defs import AutoScalingConfigurationTypeDef
 
-    data: AutoScalingConfigurationTypeDef = {...}
+    data: AutoScalingConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ChangesetStatusType,
     ChangeTypeType,
     EnvironmentStatusType,
     ErrorDetailsType,
     FederationModeType,
@@ -40,92 +40,99 @@
 __all__ = (
     "AutoScalingConfigurationTypeDef",
     "CapacityConfigurationTypeDef",
     "ChangeRequestTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
-    "CreateEnvironmentResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
-    "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
-    "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
-    "CreateKxUserResponseTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
+    "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
-    "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
-    "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
     "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
-    "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
+    "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
     "ListKxClustersRequestRequestTypeDef",
     "ListKxDatabasesRequestRequestTypeDef",
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
-    "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
-    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
-    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "CreateKxDatabaseResponseTypeDef",
+    "CreateKxEnvironmentResponseTypeDef",
+    "CreateKxUserResponseTypeDef",
+    "GetKxConnectionStringResponseTypeDef",
+    "GetKxDatabaseResponseTypeDef",
+    "GetKxUserResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateKxDatabaseResponseTypeDef",
+    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
+    "VpcConfigurationUnionTypeDef",
+    "EnvironmentTypeDef",
+    "FederationParametersUnionTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
+    "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
-    "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
+    "KxDatabaseConfigurationUnionTypeDef",
+    "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
@@ -193,21 +200,22 @@
     {
         "emailAddress": str,
         "firstName": str,
         "lastName": str,
     },
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "environmentArn": str,
-        "environmentUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "errorMessage": str,
@@ -248,14 +256,25 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "vpcId": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "ipAddressType": Literal["IP_V4"],
+    },
+    total=False,
+)
+
 _RequiredCreateKxDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -270,27 +289,14 @@
 )
 
 class CreateKxDatabaseRequestRequestTypeDef(
     _RequiredCreateKxDatabaseRequestRequestTypeDef, _OptionalCreateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
-CreateKxDatabaseResponseTypeDef = TypedDict(
-    "CreateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxEnvironmentRequestRequestTypeDef",
     {
         "name": str,
         "kmsKeyId": str,
     },
 )
@@ -306,28 +312,14 @@
 
 class CreateKxEnvironmentRequestRequestTypeDef(
     _RequiredCreateKxEnvironmentRequestRequestTypeDef,
     _OptionalCreateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-CreateKxEnvironmentResponseTypeDef = TypedDict(
-    "CreateKxEnvironmentResponseTypeDef",
-    {
-        "name": str,
-        "status": EnvironmentStatusType,
-        "environmentId": str,
-        "description": str,
-        "environmentArn": str,
-        "kmsKeyId": str,
-        "creationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -342,25 +334,14 @@
 )
 
 class CreateKxUserRequestRequestTypeDef(
     _RequiredCreateKxUserRequestRequestTypeDef, _OptionalCreateKxUserRequestRequestTypeDef
 ):
     pass
 
-CreateKxUserResponseTypeDef = TypedDict(
-    "CreateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -412,14 +393,27 @@
     "DeleteKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
+FederationParametersOutputTypeDef = TypedDict(
+    "FederationParametersOutputTypeDef",
+    {
+        "samlMetadataDocument": str,
+        "samlMetadataURL": str,
+        "applicationCallBackURL": str,
+        "federationURN": str,
+        "federationProviderName": str,
+        "attributeMap": Dict[str, str],
+    },
+    total=False,
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -445,47 +439,22 @@
     {
         "userArn": str,
         "environmentId": str,
         "clusterName": str,
     },
 )
 
-GetKxConnectionStringResponseTypeDef = TypedDict(
-    "GetKxConnectionStringResponseTypeDef",
-    {
-        "signedConnectionString": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxDatabaseRequestRequestTypeDef = TypedDict(
     "GetKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
     },
 )
 
-GetKxDatabaseResponseTypeDef = TypedDict(
-    "GetKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "lastCompletedChangesetId": str,
-        "numBytes": int,
-        "numChangesets": int,
-        "numFiles": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -501,25 +470,14 @@
     "GetKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
-GetKxUserResponseTypeDef = TypedDict(
-    "GetKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KxChangesetListEntryTypeDef = TypedDict(
     "KxChangesetListEntryTypeDef",
     {
         "changesetId": str,
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
@@ -543,14 +501,22 @@
         "availabilityZoneId": str,
         "lastModifiedTimestamp": datetime,
         "createdTimestamp": datetime,
     },
     total=False,
 )
 
+KxDatabaseCacheConfigurationOutputTypeDef = TypedDict(
+    "KxDatabaseCacheConfigurationOutputTypeDef",
+    {
+        "cacheType": str,
+        "dbPaths": List[str],
+    },
+)
+
 KxDatabaseCacheConfigurationTypeDef = TypedDict(
     "KxDatabaseCacheConfigurationTypeDef",
     {
         "cacheType": str,
         "dbPaths": Sequence[str],
     },
 )
@@ -676,18 +642,20 @@
 )
 
 class ListKxDatabasesRequestRequestTypeDef(
     _RequiredListKxDatabasesRequestRequestTypeDef, _OptionalListKxDatabasesRequestRequestTypeDef
 ):
     pass
 
-ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
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
 
 ListKxEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListKxEnvironmentsRequestRequestTypeDef",
     {
@@ -720,43 +688,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -786,25 +725,14 @@
 )
 
 class UpdateKxDatabaseRequestRequestTypeDef(
     _RequiredUpdateKxDatabaseRequestRequestTypeDef, _OptionalUpdateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
-UpdateKxDatabaseResponseTypeDef = TypedDict(
-    "UpdateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "environmentId": str,
-        "description": str,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
@@ -840,54 +768,24 @@
 )
 
 class UpdateKxUserRequestRequestTypeDef(
     _RequiredUpdateKxUserRequestRequestTypeDef, _OptionalUpdateKxUserRequestRequestTypeDef
 ):
     pass
 
-UpdateKxUserResponseTypeDef = TypedDict(
-    "UpdateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKxChangesetRequestRequestTypeDef = TypedDict(
     "CreateKxChangesetRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
     },
 )
 
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "name": str,
-        "environmentId": str,
-        "awsAccountId": str,
-        "status": EnvironmentStatusType,
-        "environmentUrl": str,
-        "description": str,
-        "environmentArn": str,
-        "sageMakerStudioDomainUrl": str,
-        "kmsKeyId": str,
-        "dedicatedServiceAccountId": str,
-        "federationMode": FederationModeType,
-        "federationParameters": FederationParametersTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -927,26 +825,140 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "environmentArn": str,
+        "environmentUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxDatabaseResponseTypeDef = TypedDict(
+    "CreateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxEnvironmentResponseTypeDef = TypedDict(
+    "CreateKxEnvironmentResponseTypeDef",
+    {
+        "name": str,
+        "status": EnvironmentStatusType,
+        "environmentId": str,
+        "description": str,
+        "environmentArn": str,
+        "kmsKeyId": str,
+        "creationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxUserResponseTypeDef = TypedDict(
+    "CreateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxConnectionStringResponseTypeDef = TypedDict(
+    "GetKxConnectionStringResponseTypeDef",
+    {
+        "signedConnectionString": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxDatabaseResponseTypeDef = TypedDict(
+    "GetKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "lastCompletedChangesetId": str,
+        "numBytes": int,
+        "numChangesets": int,
+        "numFiles": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxUserResponseTypeDef = TypedDict(
+    "GetKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
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
+UpdateKxDatabaseResponseTypeDef = TypedDict(
+    "UpdateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "environmentId": str,
+        "description": str,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKxUserResponseTypeDef = TypedDict(
+    "UpdateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
@@ -954,18 +966,41 @@
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "name": str,
+        "environmentId": str,
+        "awsAccountId": str,
+        "status": EnvironmentStatusType,
+        "environmentUrl": str,
+        "description": str,
+        "environmentArn": str,
+        "sageMakerStudioDomainUrl": str,
+        "kmsKeyId": str,
+        "dedicatedServiceAccountId": str,
+        "federationMode": FederationModeType,
+        "federationParameters": FederationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+FederationParametersUnionTypeDef = Union[
+    FederationParametersTypeDef, FederationParametersOutputTypeDef
+]
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -978,15 +1013,15 @@
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KxEnvironmentTypeDef = TypedDict(
     "KxEnvironmentTypeDef",
     {
         "name": str,
@@ -1047,15 +1082,15 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKxEnvironmentResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1070,36 +1105,56 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxChangesetsResponseTypeDef = TypedDict(
     "ListKxChangesetsResponseTypeDef",
     {
         "kxChangesets": List[KxChangesetListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClustersResponseTypeDef = TypedDict(
     "ListKxClustersResponseTypeDef",
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKxDatabaseConfigurationOutputTypeDef",
+    {
+        "databaseName": str,
+    },
+)
+_OptionalKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKxDatabaseConfigurationOutputTypeDef",
+    {
+        "cacheConfigurations": List[KxDatabaseCacheConfigurationOutputTypeDef],
+        "changesetId": str,
+    },
+    total=False,
+)
+
+class KxDatabaseConfigurationOutputTypeDef(
+    _RequiredKxDatabaseConfigurationOutputTypeDef, _OptionalKxDatabaseConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
     },
 )
 _OptionalKxDatabaseConfigurationTypeDef = TypedDict(
@@ -1117,167 +1172,178 @@
     pass
 
 ListKxDatabasesResponseTypeDef = TypedDict(
     "ListKxDatabasesResponseTypeDef",
     {
         "kxDatabases": List[KxDatabaseListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClusterNodesResponseTypeDef = TypedDict(
     "ListKxClusterNodesResponseTypeDef",
     {
         "nodes": List[KxNodeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxUsersResponseTypeDef = TypedDict(
     "ListKxUsersResponseTypeDef",
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxEnvironmentsResponseTypeDef = TypedDict(
     "ListKxEnvironmentsResponseTypeDef",
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKxClusterRequestRequestTypeDef",
+CreateKxClusterResponseTypeDef = TypedDict(
+    "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
+        "status": KxClusterStatusType,
+        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
-        "releaseLabel": str,
-        "azMode": KxAzModeType,
-    },
-)
-_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKxClusterRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
+        "releaseLabel": str,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
+        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "tags": Mapping[str, str],
+        "createdTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateKxClusterRequestRequestTypeDef(
-    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
-):
-    pass
-
-CreateKxClusterResponseTypeDef = TypedDict(
-    "CreateKxClusterResponseTypeDef",
+GetKxClusterResponseTypeDef = TypedDict(
+    "GetKxClusterResponseTypeDef",
     {
-        "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
         "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
         "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetKxClusterResponseTypeDef = TypedDict(
-    "GetKxClusterResponseTypeDef",
+KxDatabaseConfigurationUnionTypeDef = Union[
+    KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef
+]
+_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
-        "status": KxClusterStatusType,
-        "statusReason": str,
+        "environmentId": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
+        "azMode": KxAzModeType,
+    },
+)
+_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKxClusterRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
+        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
-        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
-        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+class CreateKxClusterRequestRequestTypeDef(
+    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/PKG-INFO` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore finspace type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore finspace type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-finspace"></a>
 
 # types-aiobotocore-finspace
 
 [![PyPI - types-aiobotocore-finspace](https://img.shields.io/pypi/v/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-finspace?color=blue)](https://pypistats.org/packages/types-aiobotocore-finspace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.finspace 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [types-aiobotocore-finspace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/).
 
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
@@ -319,112 +318,119 @@
 )
 
 
 def check_value(value: AutoScalingMetricType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_finspace.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    CreateEnvironmentResponseTypeDef,
+    ResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
+    VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
-    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
-    CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
+    FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
-    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
-    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
     TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
-    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
+    KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    CreateKxDatabaseResponseTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
+    CreateKxUserResponseTypeDef,
+    GetKxConnectionStringResponseTypeDef,
+    GetKxDatabaseResponseTypeDef,
+    GetKxUserResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    VpcConfigurationUnionTypeDef,
+    EnvironmentTypeDef,
+    FederationParametersUnionTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
-    CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
+    CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_value() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-finspace-2.5.2/types_aiobotocore_finspace.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*


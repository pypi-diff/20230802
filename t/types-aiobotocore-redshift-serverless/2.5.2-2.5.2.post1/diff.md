# Comparing `tmp/types-aiobotocore-redshift-serverless-2.5.2.tar.gz` & `tmp/types-aiobotocore-redshift-serverless-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-serverless-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-serverless-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-redshift-serverless-2.5.2.tar` & `types-aiobotocore-redshift-serverless-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.266760 types-aiobotocore-redshift-serverless-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-08 01:44:11.262760 types-aiobotocore-redshift-serverless-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.266760 types-aiobotocore-redshift-serverless-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.258760 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35111 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33830 2023-07-08 01:39:07.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-07-08 01:39:07.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:06.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.262760 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.337483 types-aiobotocore-redshift-serverless-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-08-02 14:52:52.329483 types-aiobotocore-redshift-serverless-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.337483 types-aiobotocore-redshift-serverless-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.329483 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35080 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33772 2023-08-02 14:47:45.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.329483 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/LICENSE` & `types-aiobotocore-redshift-serverless-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/PKG-INFO` & `types-aiobotocore-redshift-serverless-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-serverless
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore redshift-serverless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift-serverless"></a>
 
 # types-aiobotocore-redshift-serverless
 
 [![PyPI - types-aiobotocore-redshift-serverless](https://img.shields.io/pypi/v/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift-serverless?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RedshiftServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [types-aiobotocore-redshift-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/).
 
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
@@ -340,84 +339,77 @@
 )
 
 
 def check_value(value: ListEndpointAccessPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift_serverless.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListSnapshotsRequestRequestTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    TimestampTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -435,14 +427,23 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListSnapshotsRequestRequestTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -452,15 +453,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_value() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/README.md` & `types-aiobotocore-redshift-serverless-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-redshift-serverless"></a>
 
 # types-aiobotocore-redshift-serverless
 
 [![PyPI - types-aiobotocore-redshift-serverless](https://img.shields.io/pypi/v/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift-serverless?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RedshiftServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [types-aiobotocore-redshift-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/).
 
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
@@ -307,84 +307,77 @@
 )
 
 
 def check_value(value: ListEndpointAccessPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift_serverless.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListSnapshotsRequestRequestTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    TimestampTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -402,14 +395,23 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListSnapshotsRequestRequestTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -419,15 +421,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_value() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/setup.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-serverless",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore redshift-serverless type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore redshift-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_redshift_serverless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/__init__.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/__init__.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/__main__.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RedshiftServerless 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.RedshiftServerless 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/client.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("redshift-serverless") as client:
         client: RedshiftServerlessClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     LogExportType,
     UsageLimitBreachActionType,
@@ -67,14 +66,15 @@
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreFromRecoveryPointResponseTypeDef,
     RestoreFromSnapshotResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateEndpointAccessResponseTypeDef,
     UpdateNamespaceResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     UpdateUsageLimitResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
@@ -417,38 +417,38 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_namespaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_namespaces)
         """
 
     async def list_recovery_points(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListRecoveryPointsResponseTypeDef:
         """
         Returns an array of recovery points.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_recovery_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_recovery_points)
         """
 
     async def list_snapshots(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListSnapshotsResponseTypeDef:
         """
         Returns a list of snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_snapshots)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/client.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("redshift-serverless") as client:
         client: RedshiftServerlessClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     LogExportType,
     UsageLimitBreachActionType,
@@ -67,14 +66,15 @@
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreFromRecoveryPointResponseTypeDef,
     RestoreFromSnapshotResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateEndpointAccessResponseTypeDef,
     UpdateNamespaceResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     UpdateUsageLimitResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
@@ -386,37 +386,37 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_namespaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_namespaces)
         """
     async def list_recovery_points(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListRecoveryPointsResponseTypeDef:
         """
         Returns an array of recovery points.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_recovery_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_recovery_points)
         """
     async def list_snapshots(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListSnapshotsResponseTypeDef:
         """
         Returns a list of snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_snapshots)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/literals.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/literals.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/paginator.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,30 @@
         list_recovery_points_paginator: ListRecoveryPointsPaginator = client.get_paginator("list_recovery_points")
         list_snapshots_paginator: ListSnapshotsPaginator = client.get_paginator("list_snapshots")
         list_table_restore_status_paginator: ListTableRestoreStatusPaginator = client.get_paginator("list_table_restore_status")
         list_usage_limits_paginator: ListUsageLimitsPaginator = client.get_paginator("list_usage_limits")
         list_workgroups_paginator: ListWorkgroupsPaginator = client.get_paginator("list_workgroups")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import UsageLimitUsageTypeType
 from .type_defs import (
     ListEndpointAccessResponseTypeDef,
     ListNamespacesResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListEndpointAccessPaginator",
     "ListNamespacesPaginator",
     "ListRecoveryPointsPaginator",
     "ListSnapshotsPaginator",
@@ -78,30 +78,30 @@
     """
 
     def paginate(
         self,
         *,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
 
 class ListNamespacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listnamespacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listnamespacespaginator)
         """
 
 
@@ -110,19 +110,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listrecoverypointspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
 
@@ -131,20 +131,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
 
@@ -155,15 +155,15 @@
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
 
@@ -174,28 +174,28 @@
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
 
 class ListWorkgroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listworkgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkgroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listworkgroupspaginator)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/paginator.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,30 @@
         list_recovery_points_paginator: ListRecoveryPointsPaginator = client.get_paginator("list_recovery_points")
         list_snapshots_paginator: ListSnapshotsPaginator = client.get_paginator("list_snapshots")
         list_table_restore_status_paginator: ListTableRestoreStatusPaginator = client.get_paginator("list_table_restore_status")
         list_usage_limits_paginator: ListUsageLimitsPaginator = client.get_paginator("list_usage_limits")
         list_workgroups_paginator: ListWorkgroupsPaginator = client.get_paginator("list_workgroups")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import UsageLimitUsageTypeType
 from .type_defs import (
     ListEndpointAccessResponseTypeDef,
     ListNamespacesResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListEndpointAccessPaginator",
     "ListNamespacesPaginator",
     "ListRecoveryPointsPaginator",
     "ListSnapshotsPaginator",
@@ -75,29 +75,29 @@
     """
 
     def paginate(
         self,
         *,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
 class ListNamespacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listnamespacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listnamespacespaginator)
         """
 
 class ListRecoveryPointsPaginator(AioPaginator):
@@ -105,19 +105,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listrecoverypointspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
 class ListSnapshotsPaginator(AioPaginator):
@@ -125,20 +125,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
 class ListTableRestoreStatusPaginator(AioPaginator):
@@ -148,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
 class ListUsageLimitsPaginator(AioPaginator):
@@ -166,27 +166,27 @@
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
 class ListWorkgroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listworkgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkgroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listworkgroupspaginator)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/type_defs.py` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_redshift_serverless.type_defs import ConfigParameterTypeDef
 
-    data: ConfigParameterTypeDef = {...}
+    data: ConfigParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -30,73 +30,65 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ConfigParameterTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
     "UsageLimitTypeDef",
     "DeleteEndpointAccessRequestRequestTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteUsageLimitRequestRequestTypeDef",
     "DeleteWorkgroupRequestRequestTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "GetCredentialsRequestRequestTypeDef",
-    "GetCredentialsResponseTypeDef",
     "GetEndpointAccessRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetRecoveryPointRequestRequestTypeDef",
     "RecoveryPointTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    "ListRecoveryPointsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    "ListSnapshotsRequestRequestTypeDef",
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    "TimestampTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetCredentialsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -114,14 +106,23 @@
     "GetRecoveryPointResponseTypeDef",
     "ListRecoveryPointsResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    "ListRecoveryPointsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListSnapshotsRequestRequestTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -147,14 +148,25 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
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
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "accountsWithProvisionedRestoreAccess": List[str],
         "accountsWithRestoreAccess": List[str],
         "actualIncrementalBackupSizeInMegaBytes": float,
         "adminUsername": str,
@@ -342,25 +354,14 @@
 
 class GetCredentialsRequestRequestTypeDef(
     _RequiredGetCredentialsRequestRequestTypeDef, _OptionalGetCredentialsRequestRequestTypeDef
 ):
     pass
 
 
-GetCredentialsResponseTypeDef = TypedDict(
-    "GetCredentialsResponseTypeDef",
-    {
-        "dbPassword": str,
-        "dbUser": str,
-        "expiration": datetime,
-        "nextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEndpointAccessRequestRequestTypeDef = TypedDict(
     "GetEndpointAccessRequestRequestTypeDef",
     {
         "endpointName": str,
     },
 )
 
@@ -456,20 +457,20 @@
 GetWorkgroupRequestRequestTypeDef = TypedDict(
     "GetWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 
-ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "vpcId": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEndpointAccessRequestRequestTypeDef = TypedDict(
     "ListEndpointAccessRequestRequestTypeDef",
     {
@@ -477,93 +478,24 @@
         "nextToken": str,
         "vpcId": str,
         "workgroupName": str,
     },
     total=False,
 )
 
-ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRecoveryPointsRequestRequestTypeDef = TypedDict(
-    "ListRecoveryPointsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSnapshotsRequestRequestTypeDef = TypedDict(
-    "ListSnapshotsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    {
-        "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -574,43 +506,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
     },
     total=False,
 )
 
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkgroupsRequestRequestTypeDef = TypedDict(
     "ListWorkgroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -623,43 +537,22 @@
         "networkInterfaceId": str,
         "privateIpAddress": str,
         "subnetId": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 RestoreFromRecoveryPointRequestRequestTypeDef = TypedDict(
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     {
         "namespaceName": str,
         "recoveryPointId": str,
         "workgroupName": str,
     },
@@ -946,236 +839,345 @@
 
 class CreateWorkgroupRequestRequestTypeDef(
     _RequiredCreateWorkgroupRequestRequestTypeDef, _OptionalCreateWorkgroupRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+GetCredentialsResponseTypeDef = TypedDict(
+    "GetCredentialsResponseTypeDef",
+    {
+        "dbPassword": str,
+        "dbUser": str,
+        "expiration": datetime,
+        "nextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResponseTypeDef = TypedDict(
     "GetSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSnapshotsResponseTypeDef = TypedDict(
     "ListSnapshotsResponseTypeDef",
     {
         "nextToken": str,
         "snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNamespaceResponseTypeDef = TypedDict(
     "CreateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNamespaceResponseTypeDef = TypedDict(
     "DeleteNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "namespaces": List[NamespaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromRecoveryPointResponseTypeDef = TypedDict(
     "RestoreFromRecoveryPointResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "recoveryPointId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromSnapshotResponseTypeDef = TypedDict(
     "RestoreFromSnapshotResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "ownerAccount": str,
         "snapshotName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNamespaceResponseTypeDef = TypedDict(
     "UpdateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUsageLimitResponseTypeDef = TypedDict(
     "CreateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteUsageLimitResponseTypeDef = TypedDict(
     "DeleteUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageLimitResponseTypeDef = TypedDict(
     "GetUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageLimitsResponseTypeDef = TypedDict(
     "ListUsageLimitsResponseTypeDef",
     {
         "nextToken": str,
         "usageLimits": List[UsageLimitTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUsageLimitResponseTypeDef = TypedDict(
     "UpdateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecoveryPointResponseTypeDef = TypedDict(
     "GetRecoveryPointResponseTypeDef",
     {
         "recoveryPoint": RecoveryPointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsResponseTypeDef = TypedDict(
     "ListRecoveryPointsResponseTypeDef",
     {
         "nextToken": str,
         "recoveryPoints": List[RecoveryPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcePolicyResponseTypeDef = TypedDict(
     "GetResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTableRestoreStatusResponseTypeDef = TypedDict(
     "GetTableRestoreStatusResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableRestoreStatusResponseTypeDef = TypedDict(
     "ListTableRestoreStatusResponseTypeDef",
     {
         "nextToken": str,
         "tableRestoreStatuses": List[TableRestoreStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromSnapshotResponseTypeDef = TypedDict(
     "RestoreTableFromSnapshotResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    {
+        "vpcId": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    {
+        "namespaceName": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "startTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestRequestTypeDef = TypedDict(
+    "ListRecoveryPointsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSnapshotsRequestRequestTypeDef = TypedDict(
+    "ListSnapshotsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "nextToken": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "vpcEndpointId": str,
@@ -1211,48 +1213,48 @@
     total=False,
 )
 
 CreateEndpointAccessResponseTypeDef = TypedDict(
     "CreateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEndpointAccessResponseTypeDef = TypedDict(
     "DeleteEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEndpointAccessResponseTypeDef = TypedDict(
     "GetEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointAccessResponseTypeDef = TypedDict(
     "ListEndpointAccessResponseTypeDef",
     {
         "endpoints": List[EndpointAccessTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointAccessResponseTypeDef = TypedDict(
     "UpdateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
@@ -1273,43 +1275,43 @@
     total=False,
 )
 
 CreateWorkgroupResponseTypeDef = TypedDict(
     "CreateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteWorkgroupResponseTypeDef = TypedDict(
     "DeleteWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkgroupResponseTypeDef = TypedDict(
     "GetWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkgroupsResponseTypeDef = TypedDict(
     "ListWorkgroupsResponseTypeDef",
     {
         "nextToken": str,
         "workgroups": List[WorkgroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkgroupResponseTypeDef = TypedDict(
     "UpdateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless/type_defs.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_redshift_serverless.type_defs import ConfigParameterTypeDef
 
-    data: ConfigParameterTypeDef = {...}
+    data: ConfigParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -29,73 +29,65 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ConfigParameterTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
     "UsageLimitTypeDef",
     "DeleteEndpointAccessRequestRequestTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteUsageLimitRequestRequestTypeDef",
     "DeleteWorkgroupRequestRequestTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "GetCredentialsRequestRequestTypeDef",
-    "GetCredentialsResponseTypeDef",
     "GetEndpointAccessRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetRecoveryPointRequestRequestTypeDef",
     "RecoveryPointTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    "ListRecoveryPointsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    "ListSnapshotsRequestRequestTypeDef",
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    "TimestampTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetCredentialsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -113,14 +105,23 @@
     "GetRecoveryPointResponseTypeDef",
     "ListRecoveryPointsResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    "ListRecoveryPointsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListSnapshotsRequestRequestTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -146,14 +147,25 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
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
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "accountsWithProvisionedRestoreAccess": List[str],
         "accountsWithRestoreAccess": List[str],
         "actualIncrementalBackupSizeInMegaBytes": float,
         "adminUsername": str,
@@ -333,25 +345,14 @@
 )
 
 class GetCredentialsRequestRequestTypeDef(
     _RequiredGetCredentialsRequestRequestTypeDef, _OptionalGetCredentialsRequestRequestTypeDef
 ):
     pass
 
-GetCredentialsResponseTypeDef = TypedDict(
-    "GetCredentialsResponseTypeDef",
-    {
-        "dbPassword": str,
-        "dbUser": str,
-        "expiration": datetime,
-        "nextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEndpointAccessRequestRequestTypeDef = TypedDict(
     "GetEndpointAccessRequestRequestTypeDef",
     {
         "endpointName": str,
     },
 )
 
@@ -447,20 +448,20 @@
 GetWorkgroupRequestRequestTypeDef = TypedDict(
     "GetWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 
-ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "vpcId": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEndpointAccessRequestRequestTypeDef = TypedDict(
     "ListEndpointAccessRequestRequestTypeDef",
     {
@@ -468,93 +469,24 @@
         "nextToken": str,
         "vpcId": str,
         "workgroupName": str,
     },
     total=False,
 )
 
-ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRecoveryPointsRequestRequestTypeDef = TypedDict(
-    "ListRecoveryPointsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSnapshotsRequestRequestTypeDef = TypedDict(
-    "ListSnapshotsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    {
-        "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -565,43 +497,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
     },
     total=False,
 )
 
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkgroupsRequestRequestTypeDef = TypedDict(
     "ListWorkgroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -614,43 +528,22 @@
         "networkInterfaceId": str,
         "privateIpAddress": str,
         "subnetId": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 RestoreFromRecoveryPointRequestRequestTypeDef = TypedDict(
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     {
         "namespaceName": str,
         "recoveryPointId": str,
         "workgroupName": str,
     },
@@ -915,236 +808,345 @@
 )
 
 class CreateWorkgroupRequestRequestTypeDef(
     _RequiredCreateWorkgroupRequestRequestTypeDef, _OptionalCreateWorkgroupRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+GetCredentialsResponseTypeDef = TypedDict(
+    "GetCredentialsResponseTypeDef",
+    {
+        "dbPassword": str,
+        "dbUser": str,
+        "expiration": datetime,
+        "nextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResponseTypeDef = TypedDict(
     "GetSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSnapshotsResponseTypeDef = TypedDict(
     "ListSnapshotsResponseTypeDef",
     {
         "nextToken": str,
         "snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNamespaceResponseTypeDef = TypedDict(
     "CreateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNamespaceResponseTypeDef = TypedDict(
     "DeleteNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "namespaces": List[NamespaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromRecoveryPointResponseTypeDef = TypedDict(
     "RestoreFromRecoveryPointResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "recoveryPointId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromSnapshotResponseTypeDef = TypedDict(
     "RestoreFromSnapshotResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "ownerAccount": str,
         "snapshotName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNamespaceResponseTypeDef = TypedDict(
     "UpdateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUsageLimitResponseTypeDef = TypedDict(
     "CreateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteUsageLimitResponseTypeDef = TypedDict(
     "DeleteUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageLimitResponseTypeDef = TypedDict(
     "GetUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageLimitsResponseTypeDef = TypedDict(
     "ListUsageLimitsResponseTypeDef",
     {
         "nextToken": str,
         "usageLimits": List[UsageLimitTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUsageLimitResponseTypeDef = TypedDict(
     "UpdateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecoveryPointResponseTypeDef = TypedDict(
     "GetRecoveryPointResponseTypeDef",
     {
         "recoveryPoint": RecoveryPointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsResponseTypeDef = TypedDict(
     "ListRecoveryPointsResponseTypeDef",
     {
         "nextToken": str,
         "recoveryPoints": List[RecoveryPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcePolicyResponseTypeDef = TypedDict(
     "GetResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTableRestoreStatusResponseTypeDef = TypedDict(
     "GetTableRestoreStatusResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableRestoreStatusResponseTypeDef = TypedDict(
     "ListTableRestoreStatusResponseTypeDef",
     {
         "nextToken": str,
         "tableRestoreStatuses": List[TableRestoreStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromSnapshotResponseTypeDef = TypedDict(
     "RestoreTableFromSnapshotResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    {
+        "vpcId": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    {
+        "namespaceName": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "startTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestRequestTypeDef = TypedDict(
+    "ListRecoveryPointsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSnapshotsRequestRequestTypeDef = TypedDict(
+    "ListSnapshotsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "nextToken": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "vpcEndpointId": str,
@@ -1180,48 +1182,48 @@
     total=False,
 )
 
 CreateEndpointAccessResponseTypeDef = TypedDict(
     "CreateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEndpointAccessResponseTypeDef = TypedDict(
     "DeleteEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEndpointAccessResponseTypeDef = TypedDict(
     "GetEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointAccessResponseTypeDef = TypedDict(
     "ListEndpointAccessResponseTypeDef",
     {
         "endpoints": List[EndpointAccessTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointAccessResponseTypeDef = TypedDict(
     "UpdateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
@@ -1242,43 +1244,43 @@
     total=False,
 )
 
 CreateWorkgroupResponseTypeDef = TypedDict(
     "CreateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteWorkgroupResponseTypeDef = TypedDict(
     "DeleteWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkgroupResponseTypeDef = TypedDict(
     "GetWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkgroupsResponseTypeDef = TypedDict(
     "ListWorkgroupsResponseTypeDef",
     {
         "nextToken": str,
         "workgroups": List[WorkgroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkgroupResponseTypeDef = TypedDict(
     "UpdateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-serverless
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore redshift-serverless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift-serverless"></a>
 
 # types-aiobotocore-redshift-serverless
 
 [![PyPI - types-aiobotocore-redshift-serverless](https://img.shields.io/pypi/v/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift-serverless?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RedshiftServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [types-aiobotocore-redshift-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/).
 
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
@@ -340,84 +339,77 @@
 )
 
 
 def check_value(value: ListEndpointAccessPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift_serverless.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListSnapshotsRequestRequestTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    TimestampTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -435,14 +427,23 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListSnapshotsRequestRequestTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -452,15 +453,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_value() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*


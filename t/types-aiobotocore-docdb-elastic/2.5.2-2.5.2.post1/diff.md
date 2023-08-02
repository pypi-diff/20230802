# Comparing `tmp/types-aiobotocore-docdb-elastic-2.5.2.tar.gz` & `tmp/types-aiobotocore-docdb-elastic-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-elastic-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-elastic-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:11 2023, max compression
```

## Comparing `types-aiobotocore-docdb-elastic-2.5.2.tar` & `types-aiobotocore-docdb-elastic-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.953601 types-aiobotocore-docdb-elastic-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-08-02 14:52:11.949601 types-aiobotocore-docdb-elastic-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:11.953601 types-aiobotocore-docdb-elastic-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.933601 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.949601 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/LICENSE` & `types-aiobotocore-docdb-elastic-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore docdb-elastic type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore docdb-elastic type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-docdb-elastic"></a>
 
 # types-aiobotocore-docdb-elastic
 
 [![PyPI - types-aiobotocore-docdb-elastic](https://img.shields.io/pypi/v/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb-elastic?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb-elastic)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb-elastic)](https://pepy.tech/project/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DocDBElastic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
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
@@ -313,59 +312,59 @@
 )
 
 
 def check_value(value: AuthType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_docdb_elastic.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    ListClustersOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
     CreateClusterOutputTypeDef,
+    CreateClusterSnapshotOutputTypeDef,
     DeleteClusterOutputTypeDef,
+    DeleteClusterSnapshotOutputTypeDef,
     GetClusterOutputTypeDef,
+    GetClusterSnapshotOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
-def get_structure() -> ClusterInListTypeDef:
+def get_value() -> ClusterInListTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/README.md` & `types-aiobotocore-docdb-elastic-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-docdb-elastic"></a>
 
 # types-aiobotocore-docdb-elastic
 
 [![PyPI - types-aiobotocore-docdb-elastic](https://img.shields.io/pypi/v/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb-elastic?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb-elastic)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb-elastic)](https://pepy.tech/project/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DocDBElastic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
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
@@ -280,59 +280,59 @@
 )
 
 
 def check_value(value: AuthType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_docdb_elastic.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    ListClustersOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
     CreateClusterOutputTypeDef,
+    CreateClusterSnapshotOutputTypeDef,
     DeleteClusterOutputTypeDef,
+    DeleteClusterSnapshotOutputTypeDef,
     GetClusterOutputTypeDef,
+    GetClusterSnapshotOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
-def get_structure() -> ClusterInListTypeDef:
+def get_value() -> ClusterInListTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/setup.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb-elastic",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_docdb_elastic"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with"
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
-    keywords="aiobotocore docdb-elastic type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore docdb-elastic type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_docdb_elastic": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/"
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__main__.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DocDBElastic 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DocDBElastic 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic\nOther"
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

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 class ListClusterSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclustersnapshotspaginator)
     """
 
     def paginate(
-        self, *, clusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClusterSnapshotsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclustersnapshotspaginator)
         """
 
 
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclusterspaginator)
         """
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 class ListClusterSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclustersnapshotspaginator)
     """
 
     def paginate(
-        self, *, clusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClusterSnapshotsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclustersnapshotspaginator)
         """
 
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/paginators/#listclusterspaginator)
         """
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.py` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_docdb_elastic.type_defs import ClusterInListTypeDef
 
-    data: ClusterInListTypeDef = {...}
+    data: ClusterInListTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import AuthType, StatusType
 
@@ -24,41 +24,41 @@
 
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateClusterSnapshotInputRequestTypeDef",
     "DeleteClusterInputRequestTypeDef",
     "DeleteClusterSnapshotInputRequestTypeDef",
     "GetClusterInputRequestTypeDef",
     "GetClusterSnapshotInputRequestTypeDef",
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClusterSnapshotsInputRequestTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreClusterFromSnapshotInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterInputRequestTypeDef",
-    "ListClustersOutputTypeDef",
-    "ListClusterSnapshotsOutputTypeDef",
-    "CreateClusterSnapshotOutputTypeDef",
-    "DeleteClusterSnapshotOutputTypeDef",
-    "GetClusterSnapshotOutputTypeDef",
     "CreateClusterOutputTypeDef",
+    "CreateClusterSnapshotOutputTypeDef",
     "DeleteClusterOutputTypeDef",
+    "DeleteClusterSnapshotOutputTypeDef",
     "GetClusterOutputTypeDef",
+    "GetClusterSnapshotOutputTypeDef",
+    "ListClusterSnapshotsOutputTypeDef",
+    "ListClustersOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RestoreClusterFromSnapshotOutputTypeDef",
     "UpdateClusterOutputTypeDef",
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
 )
 
 ClusterInListTypeDef = TypedDict(
     "ClusterInListTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
@@ -139,14 +139,25 @@
 
 class CreateClusterInputRequestTypeDef(
     _RequiredCreateClusterInputRequestTypeDef, _OptionalCreateClusterInputRequestTypeDef
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
+
 _RequiredCreateClusterSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotInputRequestTypeDef",
     {
         "clusterArn": str,
         "snapshotName": str,
     },
 )
@@ -190,41 +201,34 @@
 GetClusterSnapshotInputRequestTypeDef = TypedDict(
     "GetClusterSnapshotInputRequestTypeDef",
     {
         "snapshotArn": str,
     },
 )
 
-ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "clusterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListClusterSnapshotsInputRequestTypeDef = TypedDict(
     "ListClusterSnapshotsInputRequestTypeDef",
     {
         "clusterArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -233,43 +237,14 @@
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
 _RequiredRestoreClusterFromSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredRestoreClusterFromSnapshotInputRequestTypeDef",
     {
         "clusterName": str,
         "snapshotArn": str,
     },
 )
@@ -332,88 +307,113 @@
 
 class UpdateClusterInputRequestTypeDef(
     _RequiredUpdateClusterInputRequestTypeDef, _OptionalUpdateClusterInputRequestTypeDef
 ):
     pass
 
 
-ListClustersOutputTypeDef = TypedDict(
-    "ListClustersOutputTypeDef",
+CreateClusterOutputTypeDef = TypedDict(
+    "CreateClusterOutputTypeDef",
     {
-        "clusters": List[ClusterInListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListClusterSnapshotsOutputTypeDef = TypedDict(
-    "ListClusterSnapshotsOutputTypeDef",
+CreateClusterSnapshotOutputTypeDef = TypedDict(
+    "CreateClusterSnapshotOutputTypeDef",
     {
-        "nextToken": str,
-        "snapshots": List[ClusterSnapshotInListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "snapshot": ClusterSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterSnapshotOutputTypeDef = TypedDict(
-    "CreateClusterSnapshotOutputTypeDef",
+DeleteClusterOutputTypeDef = TypedDict(
+    "DeleteClusterOutputTypeDef",
     {
-        "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotOutputTypeDef = TypedDict(
     "DeleteClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetClusterOutputTypeDef = TypedDict(
+    "GetClusterOutputTypeDef",
+    {
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClusterSnapshotOutputTypeDef = TypedDict(
     "GetClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterOutputTypeDef = TypedDict(
-    "CreateClusterOutputTypeDef",
+ListClusterSnapshotsOutputTypeDef = TypedDict(
+    "ListClusterSnapshotsOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nextToken": str,
+        "snapshots": List[ClusterSnapshotInListTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteClusterOutputTypeDef = TypedDict(
-    "DeleteClusterOutputTypeDef",
+ListClustersOutputTypeDef = TypedDict(
+    "ListClustersOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "clusters": List[ClusterInListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetClusterOutputTypeDef = TypedDict(
-    "GetClusterOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreClusterFromSnapshotOutputTypeDef = TypedDict(
     "RestoreClusterFromSnapshotOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterOutputTypeDef = TypedDict(
     "UpdateClusterOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    {
+        "clusterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_docdb_elastic.type_defs import ClusterInListTypeDef
 
-    data: ClusterInListTypeDef = {...}
+    data: ClusterInListTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import AuthType, StatusType
 
@@ -23,41 +23,41 @@
 
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateClusterSnapshotInputRequestTypeDef",
     "DeleteClusterInputRequestTypeDef",
     "DeleteClusterSnapshotInputRequestTypeDef",
     "GetClusterInputRequestTypeDef",
     "GetClusterSnapshotInputRequestTypeDef",
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClusterSnapshotsInputRequestTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreClusterFromSnapshotInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterInputRequestTypeDef",
-    "ListClustersOutputTypeDef",
-    "ListClusterSnapshotsOutputTypeDef",
-    "CreateClusterSnapshotOutputTypeDef",
-    "DeleteClusterSnapshotOutputTypeDef",
-    "GetClusterSnapshotOutputTypeDef",
     "CreateClusterOutputTypeDef",
+    "CreateClusterSnapshotOutputTypeDef",
     "DeleteClusterOutputTypeDef",
+    "DeleteClusterSnapshotOutputTypeDef",
     "GetClusterOutputTypeDef",
+    "GetClusterSnapshotOutputTypeDef",
+    "ListClusterSnapshotsOutputTypeDef",
+    "ListClustersOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RestoreClusterFromSnapshotOutputTypeDef",
     "UpdateClusterOutputTypeDef",
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
 )
 
 ClusterInListTypeDef = TypedDict(
     "ClusterInListTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
@@ -136,14 +136,25 @@
 )
 
 class CreateClusterInputRequestTypeDef(
     _RequiredCreateClusterInputRequestTypeDef, _OptionalCreateClusterInputRequestTypeDef
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
+
 _RequiredCreateClusterSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotInputRequestTypeDef",
     {
         "clusterArn": str,
         "snapshotName": str,
     },
 )
@@ -185,41 +196,34 @@
 GetClusterSnapshotInputRequestTypeDef = TypedDict(
     "GetClusterSnapshotInputRequestTypeDef",
     {
         "snapshotArn": str,
     },
 )
 
-ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "clusterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListClusterSnapshotsInputRequestTypeDef = TypedDict(
     "ListClusterSnapshotsInputRequestTypeDef",
     {
         "clusterArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -228,43 +232,14 @@
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
 _RequiredRestoreClusterFromSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredRestoreClusterFromSnapshotInputRequestTypeDef",
     {
         "clusterName": str,
         "snapshotArn": str,
     },
 )
@@ -323,88 +298,113 @@
 )
 
 class UpdateClusterInputRequestTypeDef(
     _RequiredUpdateClusterInputRequestTypeDef, _OptionalUpdateClusterInputRequestTypeDef
 ):
     pass
 
-ListClustersOutputTypeDef = TypedDict(
-    "ListClustersOutputTypeDef",
+CreateClusterOutputTypeDef = TypedDict(
+    "CreateClusterOutputTypeDef",
     {
-        "clusters": List[ClusterInListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListClusterSnapshotsOutputTypeDef = TypedDict(
-    "ListClusterSnapshotsOutputTypeDef",
+CreateClusterSnapshotOutputTypeDef = TypedDict(
+    "CreateClusterSnapshotOutputTypeDef",
     {
-        "nextToken": str,
-        "snapshots": List[ClusterSnapshotInListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "snapshot": ClusterSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterSnapshotOutputTypeDef = TypedDict(
-    "CreateClusterSnapshotOutputTypeDef",
+DeleteClusterOutputTypeDef = TypedDict(
+    "DeleteClusterOutputTypeDef",
     {
-        "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotOutputTypeDef = TypedDict(
     "DeleteClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetClusterOutputTypeDef = TypedDict(
+    "GetClusterOutputTypeDef",
+    {
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClusterSnapshotOutputTypeDef = TypedDict(
     "GetClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterOutputTypeDef = TypedDict(
-    "CreateClusterOutputTypeDef",
+ListClusterSnapshotsOutputTypeDef = TypedDict(
+    "ListClusterSnapshotsOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nextToken": str,
+        "snapshots": List[ClusterSnapshotInListTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteClusterOutputTypeDef = TypedDict(
-    "DeleteClusterOutputTypeDef",
+ListClustersOutputTypeDef = TypedDict(
+    "ListClustersOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "clusters": List[ClusterInListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetClusterOutputTypeDef = TypedDict(
-    "GetClusterOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreClusterFromSnapshotOutputTypeDef = TypedDict(
     "RestoreClusterFromSnapshotOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterOutputTypeDef = TypedDict(
     "UpdateClusterOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    {
+        "clusterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore docdb-elastic type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore docdb-elastic type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-docdb-elastic"></a>
 
 # types-aiobotocore-docdb-elastic
 
 [![PyPI - types-aiobotocore-docdb-elastic](https://img.shields.io/pypi/v/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb-elastic?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb-elastic)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb-elastic)](https://pepy.tech/project/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DocDBElastic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
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
@@ -313,59 +312,59 @@
 )
 
 
 def check_value(value: AuthType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_docdb_elastic.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    ListClustersOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
     CreateClusterOutputTypeDef,
+    CreateClusterSnapshotOutputTypeDef,
     DeleteClusterOutputTypeDef,
+    DeleteClusterSnapshotOutputTypeDef,
     GetClusterOutputTypeDef,
+    GetClusterSnapshotOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
-def get_structure() -> ClusterInListTypeDef:
+def get_value() -> ClusterInListTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-ecr-public-2.5.2.tar.gz` & `tmp/types-aiobotocore-ecr-public-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-public-2.5.2.tar", last modified: Sat Jul  8 01:43:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-public-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-ecr-public-2.5.2.tar` & `types-aiobotocore-ecr-public-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-07-08 01:30:07.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.385594 types-aiobotocore-ecr-public-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-08-02 14:52:14.381594 types-aiobotocore-ecr-public-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.385594 types-aiobotocore-ecr-public-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.373594 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-08-02 14:37:54.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.381594 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/LICENSE` & `types-aiobotocore-ecr-public-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ecr-public type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ecr-public type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecr-public"></a>
 
 # types-aiobotocore-ecr-public
 
 [![PyPI - types-aiobotocore-ecr-public](https://img.shields.io/pypi/v/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr-public?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr-public)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
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
@@ -326,91 +325,92 @@
 )
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecr_public.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
+    RepositoryCatalogDataInputTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
+    CreateRepositoryRequestRequestTypeDef,
+    PutRepositoryCatalogDataRequestRequestTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationDataTypeDef:
+def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/README.md` & `types-aiobotocore-ecr-public-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ecr-public"></a>
 
 # types-aiobotocore-ecr-public
 
 [![PyPI - types-aiobotocore-ecr-public](https://img.shields.io/pypi/v/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr-public?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr-public)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
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
@@ -293,91 +293,92 @@
 )
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecr_public.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
+    RepositoryCatalogDataInputTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
+    CreateRepositoryRequestRequestTypeDef,
+    PutRepositoryCatalogDataRequestRequestTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationDataTypeDef:
+def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/setup.py` & `types-aiobotocore-ecr-public-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr-public",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore ecr-public type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ecr-public type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ecr_public": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/"
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.py` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.pyi` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__main__.py` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECRPublic 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ECRPublic 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.py` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
     session = get_session()
     async with session.create_client("ecr-public") as client:
         client: ECRPublicClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .paginator import (
     DescribeImagesPaginator,
     DescribeImageTagsPaginator,
     DescribeRegistriesPaginator,
     DescribeRepositoriesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeImagesResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
@@ -407,15 +407,15 @@
     async def upload_layer_part(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
-        layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
+        layerPartBlob: BlobTypeDef,
         registryId: str = ...
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#upload_layer_part)
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.pyi` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
     session = get_session()
     async with session.create_client("ecr-public") as client:
         client: ECRPublicClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .paginator import (
     DescribeImagesPaginator,
     DescribeImageTagsPaginator,
     DescribeRegistriesPaginator,
     DescribeRepositoriesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeImagesResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
@@ -377,15 +377,15 @@
     async def upload_layer_part(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
-        layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
+        layerPartBlob: BlobTypeDef,
         registryId: str = ...
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#upload_layer_part)
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.py` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.pyi` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.py` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 
@@ -85,30 +85,30 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagespaginator)
         """
 
 
 class DescribeRegistriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeregistriespaginator)
         """
 
 
@@ -119,13 +119,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.pyi` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 class DescribeImagesPaginator(AioPaginator):
@@ -81,29 +81,29 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagespaginator)
         """
 
 class DescribeRegistriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeregistriespaginator)
         """
 
 class DescribeRepositoriesPaginator(AioPaginator):
@@ -113,13 +113,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.py` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ecr_public.type_defs import AuthorizationDataTypeDef
 
-    data: AuthorizationDataTypeDef = {...}
+    data: AuthorizationDataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -31,72 +31,73 @@
 
 
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
-    "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
-    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
     "ImageDetailTypeDef",
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
     "DescribeRegistriesRequestRequestTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "RegistryCatalogDataTypeDef",
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
-    "PutRepositoryCatalogDataRequestRequestTypeDef",
-    "CreateRepositoryRequestRequestTypeDef",
+    "RepositoryCatalogDataInputTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
+    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
+    "CreateRepositoryRequestRequestTypeDef",
+    "PutRepositoryCatalogDataRequestRequestTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
@@ -146,23 +147,35 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
     },
     total=False,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -179,38 +192,14 @@
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RepositoryCatalogDataInputTypeDef = TypedDict(
-    "RepositoryCatalogDataInputTypeDef",
-    {
-        "description": str,
-        "architectures": Sequence[str],
-        "operatingSystems": Sequence[str],
-        "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "aboutText": str,
-        "usageText": str,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -260,24 +249,14 @@
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -292,37 +271,24 @@
 
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
-    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -353,41 +319,23 @@
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
         "artifactMediaType": str,
     },
     total=False,
 )
 
-DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRegistriesRequestRequestTypeDef = TypedDict(
     "DescribeRegistriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -443,24 +391,14 @@
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReferencedImageDetailTypeDef = TypedDict(
     "ReferencedImageDetailTypeDef",
     {
         "imageDigest": str,
         "imageSizeInBytes": int,
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
@@ -487,40 +425,21 @@
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -556,25 +475,14 @@
         "name": str,
         "status": RegistryAliasStatusType,
         "primaryRegistryAlias": bool,
         "defaultRegistryAlias": bool,
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -591,127 +499,118 @@
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_RequiredUploadLayerPartRequestRequestTypeDef",
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
     {
-        "repositoryName": str,
-        "uploadId": str,
-        "partFirstByte": int,
-        "partLastByte": int,
-        "layerPartBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_OptionalUploadLayerPartRequestRequestTypeDef",
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UploadLayerPartRequestRequestTypeDef(
-    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
-):
-    pass
-
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": AuthorizationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
     {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeleteImageRequestRequestTypeDef",
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
     {
-        "repositoryName": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeleteImageRequestRequestTypeDef",
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class BatchDeleteImageRequestRequestTypeDef(
-    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class DescribeImagesRequestDescribeImagesPaginateTypeDef(
-    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
-    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+class BatchDeleteImageRequestRequestTypeDef(
+    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
@@ -754,64 +653,57 @@
         "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
-_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-    },
-)
-_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+RepositoryCatalogDataInputTypeDef = TypedDict(
+    "RepositoryCatalogDataInputTypeDef",
     {
-        "registryId": str,
+        "description": str,
+        "architectures": Sequence[str],
+        "operatingSystems": Sequence[str],
+        "logoImageBlob": BlobTypeDef,
+        "aboutText": str,
+        "usageText": str,
     },
     total=False,
 )
 
-
-class PutRepositoryCatalogDataRequestRequestTypeDef(
-    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
-    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRepositoryRequestRequestTypeDef",
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
     },
 )
-_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRepositoryRequestRequestTypeDef",
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-        "tags": Sequence[TagTypeDef],
+        "registryId": str,
     },
     total=False,
 )
 
 
-class CreateRepositoryRequestRequestTypeDef(
-    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -819,74 +711,139 @@
     },
 )
 
 GetRepositoryCatalogDataResponseTypeDef = TypedDict(
     "GetRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryCatalogDataResponseTypeDef = TypedDict(
     "PutRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
+    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "registryId": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeImagesRequestDescribeImagesPaginateTypeDef(
+    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
+    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+):
+    pass
+
+
+DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegistryCatalogDataResponseTypeDef = TypedDict(
     "GetRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryCatalogDataResponseTypeDef = TypedDict(
     "PutRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTagDetailTypeDef = TypedDict(
     "ImageTagDetailTypeDef",
     {
         "imageTag": str,
@@ -908,36 +865,81 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRepositoryRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRepositoryRequestRequestTypeDef",
+    {
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateRepositoryRequestRequestTypeDef(
+    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+    },
+)
+_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+
+class PutRepositoryCatalogDataRequestRequestTypeDef(
+    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
+    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegistriesResponseTypeDef = TypedDict(
     "DescribeRegistriesResponseTypeDef",
     {
         "registries": List[RegistryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.pyi` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ecr_public.type_defs import AuthorizationDataTypeDef
 
-    data: AuthorizationDataTypeDef = {...}
+    data: AuthorizationDataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -30,72 +30,73 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
-    "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
-    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
     "ImageDetailTypeDef",
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
     "DescribeRegistriesRequestRequestTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "RegistryCatalogDataTypeDef",
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
-    "PutRepositoryCatalogDataRequestRequestTypeDef",
-    "CreateRepositoryRequestRequestTypeDef",
+    "RepositoryCatalogDataInputTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
+    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
+    "CreateRepositoryRequestRequestTypeDef",
+    "PutRepositoryCatalogDataRequestRequestTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
@@ -143,23 +144,35 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
     },
     total=False,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -174,38 +187,14 @@
 
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RepositoryCatalogDataInputTypeDef = TypedDict(
-    "RepositoryCatalogDataInputTypeDef",
-    {
-        "description": str,
-        "architectures": Sequence[str],
-        "operatingSystems": Sequence[str],
-        "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "aboutText": str,
-        "usageText": str,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -253,24 +242,14 @@
 
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -283,35 +262,24 @@
 )
 
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
-    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -340,41 +308,23 @@
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
         "artifactMediaType": str,
     },
     total=False,
 )
 
-DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRegistriesRequestRequestTypeDef = TypedDict(
     "DescribeRegistriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -426,24 +376,14 @@
 
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReferencedImageDetailTypeDef = TypedDict(
     "ReferencedImageDetailTypeDef",
     {
         "imageDigest": str,
         "imageSizeInBytes": int,
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
@@ -468,40 +408,21 @@
 
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -535,25 +456,14 @@
         "name": str,
         "status": RegistryAliasStatusType,
         "primaryRegistryAlias": bool,
         "defaultRegistryAlias": bool,
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -568,122 +478,117 @@
 
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_RequiredUploadLayerPartRequestRequestTypeDef",
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
     {
-        "repositoryName": str,
-        "uploadId": str,
-        "partFirstByte": int,
-        "partLastByte": int,
-        "layerPartBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_OptionalUploadLayerPartRequestRequestTypeDef",
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UploadLayerPartRequestRequestTypeDef(
-    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
-):
-    pass
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": AuthorizationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
     {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeleteImageRequestRequestTypeDef",
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
     {
-        "repositoryName": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeleteImageRequestRequestTypeDef",
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class BatchDeleteImageRequestRequestTypeDef(
-    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
-):
-    pass
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class DescribeImagesRequestDescribeImagesPaginateTypeDef(
-    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
-    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+class BatchDeleteImageRequestRequestTypeDef(
+    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -723,60 +628,55 @@
         "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
-_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-    },
-)
-_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+RepositoryCatalogDataInputTypeDef = TypedDict(
+    "RepositoryCatalogDataInputTypeDef",
     {
-        "registryId": str,
+        "description": str,
+        "architectures": Sequence[str],
+        "operatingSystems": Sequence[str],
+        "logoImageBlob": BlobTypeDef,
+        "aboutText": str,
+        "usageText": str,
     },
     total=False,
 )
 
-class PutRepositoryCatalogDataRequestRequestTypeDef(
-    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
-    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRepositoryRequestRequestTypeDef",
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
     },
 )
-_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRepositoryRequestRequestTypeDef",
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-        "tags": Sequence[TagTypeDef],
+        "registryId": str,
     },
     total=False,
 )
 
-class CreateRepositoryRequestRequestTypeDef(
-    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -784,74 +684,135 @@
     },
 )
 
 GetRepositoryCatalogDataResponseTypeDef = TypedDict(
     "GetRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryCatalogDataResponseTypeDef = TypedDict(
     "PutRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
+    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "registryId": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeImagesRequestDescribeImagesPaginateTypeDef(
+    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
+    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+):
+    pass
+
+DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegistryCatalogDataResponseTypeDef = TypedDict(
     "GetRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryCatalogDataResponseTypeDef = TypedDict(
     "PutRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTagDetailTypeDef = TypedDict(
     "ImageTagDetailTypeDef",
     {
         "imageTag": str,
@@ -873,36 +834,77 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRepositoryRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRepositoryRequestRequestTypeDef",
+    {
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+class CreateRepositoryRequestRequestTypeDef(
+    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+):
+    pass
+
+_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+    },
+)
+_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+class PutRepositoryCatalogDataRequestRequestTypeDef(
+    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
+    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
+):
+    pass
+
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegistriesResponseTypeDef = TypedDict(
     "DescribeRegistriesResponseTypeDef",
     {
         "registries": List[RegistryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ecr-public type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ecr-public type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecr-public"></a>
 
 # types-aiobotocore-ecr-public
 
 [![PyPI - types-aiobotocore-ecr-public](https://img.shields.io/pypi/v/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr-public?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr-public)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
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
@@ -326,91 +325,92 @@
 )
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecr_public.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
+    RepositoryCatalogDataInputTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
+    CreateRepositoryRequestRequestTypeDef,
+    PutRepositoryCatalogDataRequestRequestTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationDataTypeDef:
+def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*


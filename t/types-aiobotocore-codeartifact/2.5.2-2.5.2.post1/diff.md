# Comparing `tmp/types-aiobotocore-codeartifact-2.5.2.tar.gz` & `tmp/types-aiobotocore-codeartifact-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeartifact-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeartifact-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codeartifact-2.5.2.tar` & `types-aiobotocore-codeartifact-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.605865 types-aiobotocore-codeartifact-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-08 01:43:23.605865 types-aiobotocore-codeartifact-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.605865 types-aiobotocore-codeartifact-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.605865 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46955 2023-07-08 01:27:20.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46876 2023-07-08 01:27:20.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:19.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.605865 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-08 01:43:23.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:23.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:23.000000 types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.409626 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36361 2023-08-02 14:34:51.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36308 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-02 14:34:51.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46914 2023-08-02 14:34:53.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/LICENSE` & `types-aiobotocore-codeartifact-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2/PKG-INFO` & `types-aiobotocore-codeartifact-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeartifact
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeartifact type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeartifact type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeartifact"></a>
 
 # types-aiobotocore-codeartifact
 
 [![PyPI - types-aiobotocore-codeartifact](https://img.shields.io/pypi/v/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeartifact?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeartifact)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeArtifact 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [types-aiobotocore-codeartifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/).
 
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
@@ -340,25 +339,27 @@
 )
 
 
 def check_value(value: AllowPublishType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeartifact.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -373,52 +374,45 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
-    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PackageOriginRestrictionsTypeDef,
-    PaginatorConfigTypeDef,
-    PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
+    GetPackageVersionAssetResultTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
+    PublishPackageVersionRequestRequestTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -431,14 +425,20 @@
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
@@ -456,15 +456,15 @@
     ListPackageVersionsResultTypeDef,
     DescribePackageResultTypeDef,
     DeletePackageResultTypeDef,
     ListPackagesResultTypeDef,
 )
 
 
-def get_structure() -> AssetSummaryTypeDef:
+def get_value() -> AssetSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/README.md` & `types-aiobotocore-codeartifact-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codeartifact"></a>
 
 # types-aiobotocore-codeartifact
 
 [![PyPI - types-aiobotocore-codeartifact](https://img.shields.io/pypi/v/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeartifact?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeartifact)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeArtifact 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [types-aiobotocore-codeartifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/).
 
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
@@ -307,25 +307,27 @@
 )
 
 
 def check_value(value: AllowPublishType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeartifact.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -340,52 +342,45 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
-    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PackageOriginRestrictionsTypeDef,
-    PaginatorConfigTypeDef,
-    PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
+    GetPackageVersionAssetResultTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
+    PublishPackageVersionRequestRequestTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -398,14 +393,20 @@
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
@@ -423,15 +424,15 @@
     ListPackageVersionsResultTypeDef,
     DescribePackageResultTypeDef,
     DeletePackageResultTypeDef,
     ListPackagesResultTypeDef,
 )
 
 
-def get_structure() -> AssetSummaryTypeDef:
+def get_value() -> AssetSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/setup.py` & `types-aiobotocore-codeartifact-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeartifact",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with"
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
-    keywords="aiobotocore codeartifact type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codeartifact type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeartifact": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/"
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/__init__.py` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/__init__.pyi` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/__main__.py` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeArtifact 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeArtifact 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
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

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/client.py` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("codeartifact") as client:
         client: CodeArtifactClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
     PackageVersionOriginTypeType,
@@ -34,14 +33,15 @@
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
 )
 from .type_defs import (
     AssociateExternalConnectionResultTypeDef,
+    BlobTypeDef,
     CopyPackageVersionsResultTypeDef,
     CreateDomainResultTypeDef,
     CreateRepositoryResultTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteDomainResultTypeDef,
     DeletePackageResultTypeDef,
     DeletePackageVersionsResultTypeDef,
@@ -606,15 +606,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
-        assetContent: Union[str, bytes, IO[Any], StreamingBody],
+        assetContent: BlobTypeDef,
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
         unfinished: bool = ...
     ) -> PublishPackageVersionResultTypeDef:
         """
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/client.pyi` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("codeartifact") as client:
         client: CodeArtifactClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
     PackageVersionOriginTypeType,
@@ -34,14 +33,15 @@
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
 )
 from .type_defs import (
     AssociateExternalConnectionResultTypeDef,
+    BlobTypeDef,
     CopyPackageVersionsResultTypeDef,
     CreateDomainResultTypeDef,
     CreateRepositoryResultTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteDomainResultTypeDef,
     DeletePackageResultTypeDef,
     DeletePackageVersionsResultTypeDef,
@@ -568,15 +568,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
-        assetContent: Union[str, bytes, IO[Any], StreamingBody],
+        assetContent: BlobTypeDef,
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
         unfinished: bool = ...
     ) -> PublishPackageVersionResultTypeDef:
         """
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/literals.py` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/literals.pyi` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/paginator.py` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,50 +54,45 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDomainsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
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
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listdomainspaginator)
         """
 
-
 class ListPackageVersionAssetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionassetspaginator)
     """
 
     def paginate(
@@ -106,22 +101,21 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
-
 class ListPackageVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionspaginator)
     """
 
     def paginate(
@@ -132,22 +126,21 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionspaginator)
         """
 
-
 class ListPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackagespaginator)
     """
 
     def paginate(
@@ -157,49 +150,47 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackagespaginator)
         """
 
-
 class ListRepositoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, repositoryPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriespaginator)
         """
 
-
 class ListRepositoriesInDomainPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriesindomainpaginator)
     """
 
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/paginator.pyi` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,45 +54,50 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListDomainsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
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
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listdomainspaginator)
         """
 
+
 class ListPackageVersionAssetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionassetspaginator)
     """
 
     def paginate(
@@ -101,21 +106,22 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
+
 class ListPackageVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionspaginator)
     """
 
     def paginate(
@@ -126,21 +132,22 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionspaginator)
         """
 
+
 class ListPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackagespaginator)
     """
 
     def paginate(
@@ -150,47 +157,49 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackagespaginator)
         """
 
+
 class ListRepositoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, repositoryPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriespaginator)
         """
 
+
 class ListRepositoriesInDomainPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriesindomainpaginator)
     """
 
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/type_defs.py` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codeartifact.type_defs import AssetSummaryTypeDef
 
-    data: AssetSummaryTypeDef = {...}
+    data: AssetSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,18 +33,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -59,52 +60,45 @@
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
-    "GetAuthorizationTokenResultTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
-    "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
-    "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
-    "GetRepositoryEndpointResultTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
-    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PackageOriginRestrictionsTypeDef",
-    "PaginatorConfigTypeDef",
-    "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
+    "GetAuthorizationTokenResultTypeDef",
+    "GetPackageVersionAssetResultTypeDef",
+    "GetPackageVersionReadmeResultTypeDef",
+    "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
+    "PublishPackageVersionRequestRequestTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -117,14 +111,20 @@
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
@@ -156,19 +156,17 @@
     {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
     total=False,
 )
 
-
 class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
     pass
 
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -177,22 +175,32 @@
     "_OptionalAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class AssociateExternalConnectionRequestRequestTypeDef(
     _RequiredAssociateExternalConnectionRequestRequestTypeDef,
     _OptionalAssociateExternalConnectionRequestRequestTypeDef,
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
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -208,22 +216,20 @@
         "versionRevisions": Mapping[str, str],
         "allowOverwrite": bool,
         "includeFromUpstream": bool,
     },
     total=False,
 )
 
-
 class CopyPackageVersionsRequestRequestTypeDef(
     _RequiredCopyPackageVersionsRequestRequestTypeDef,
     _OptionalCopyPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
     total=False,
@@ -280,22 +286,20 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
-
 class DeleteDomainPermissionsPolicyRequestRequestTypeDef(
     _RequiredDeleteDomainPermissionsPolicyRequestRequestTypeDef,
     _OptionalDeleteDomainPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
@@ -312,21 +316,19 @@
     "_OptionalDeleteDomainRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class DeleteDomainRequestRequestTypeDef(
     _RequiredDeleteDomainRequestRequestTypeDef, _OptionalDeleteDomainRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -337,21 +339,19 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
-
 class DeletePackageRequestRequestTypeDef(
     _RequiredDeletePackageRequestRequestTypeDef, _OptionalDeletePackageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeletePackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -364,22 +364,20 @@
         "domainOwner": str,
         "namespace": str,
         "expectedStatus": PackageVersionStatusType,
     },
     total=False,
 )
 
-
 class DeletePackageVersionsRequestRequestTypeDef(
     _RequiredDeletePackageVersionsRequestRequestTypeDef,
     _OptionalDeletePackageVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -388,22 +386,20 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryPermissionsPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPermissionsPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -411,42 +407,38 @@
     "_OptionalDeleteRepositoryRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalDescribeDomainRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeDomainRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class DescribeDomainRequestRequestTypeDef(
     _RequiredDescribeDomainRequestRequestTypeDef, _OptionalDescribeDomainRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -457,21 +449,19 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
-
 class DescribePackageRequestRequestTypeDef(
     _RequiredDescribePackageRequestRequestTypeDef, _OptionalDescribePackageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribePackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -483,22 +473,20 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
-
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRepositoryRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -506,22 +494,20 @@
     "_OptionalDescribeRepositoryRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class DescribeRepositoryRequestRequestTypeDef(
     _RequiredDescribeRepositoryRequestRequestTypeDef,
     _OptionalDescribeRepositoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisassociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -530,22 +516,20 @@
     "_OptionalDisassociateExternalConnectionRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class DisassociateExternalConnectionRequestRequestTypeDef(
     _RequiredDisassociateExternalConnectionRequestRequestTypeDef,
     _OptionalDisassociateExternalConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisposePackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDisposePackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -559,22 +543,20 @@
         "namespace": str,
         "versionRevisions": Mapping[str, str],
         "expectedStatus": PackageVersionStatusType,
     },
     total=False,
 )
 
-
 class DisposePackageVersionsRequestRequestTypeDef(
     _RequiredDisposePackageVersionsRequestRequestTypeDef,
     _OptionalDisposePackageVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
     total=False,
@@ -604,53 +586,40 @@
     {
         "domainOwner": str,
         "durationSeconds": int,
     },
     total=False,
 )
 
-
 class GetAuthorizationTokenRequestRequestTypeDef(
     _RequiredGetAuthorizationTokenRequestRequestTypeDef,
     _OptionalGetAuthorizationTokenRequestRequestTypeDef,
 ):
     pass
 
-
-GetAuthorizationTokenResultTypeDef = TypedDict(
-    "GetAuthorizationTokenResultTypeDef",
-    {
-        "authorizationToken": str,
-        "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class GetDomainPermissionsPolicyRequestRequestTypeDef(
     _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef,
     _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetPackageVersionAssetRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionAssetRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -664,33 +633,20 @@
         "domainOwner": str,
         "namespace": str,
         "packageVersionRevision": str,
     },
     total=False,
 )
 
-
 class GetPackageVersionAssetRequestRequestTypeDef(
     _RequiredGetPackageVersionAssetRequestRequestTypeDef,
     _OptionalGetPackageVersionAssetRequestRequestTypeDef,
 ):
     pass
 
-
-GetPackageVersionAssetResultTypeDef = TypedDict(
-    "GetPackageVersionAssetResultTypeDef",
-    {
-        "asset": StreamingBody,
-        "assetName": str,
-        "packageVersion": str,
-        "packageVersionRevision": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPackageVersionReadmeRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionReadmeRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -702,35 +658,20 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
-
 class GetPackageVersionReadmeRequestRequestTypeDef(
     _RequiredGetPackageVersionReadmeRequestRequestTypeDef,
     _OptionalGetPackageVersionReadmeRequestRequestTypeDef,
 ):
     pass
 
-
-GetPackageVersionReadmeResultTypeDef = TypedDict(
-    "GetPackageVersionReadmeResultTypeDef",
-    {
-        "format": PackageFormatType,
-        "namespace": str,
-        "package": str,
-        "version": str,
-        "versionRevision": str,
-        "readme": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
     },
@@ -739,30 +680,20 @@
     "_OptionalGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class GetRepositoryEndpointRequestRequestTypeDef(
     _RequiredGetRepositoryEndpointRequestRequestTypeDef,
     _OptionalGetRepositoryEndpointRequestRequestTypeDef,
 ):
     pass
 
-
-GetRepositoryEndpointResultTypeDef = TypedDict(
-    "GetRepositoryEndpointResultTypeDef",
-    {
-        "repositoryEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -770,76 +701,48 @@
     "_OptionalGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
-
 class GetRepositoryPermissionsPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-    },
-)
-_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
-    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -853,22 +756,20 @@
         "namespace": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListPackageVersionAssetsRequestRequestTypeDef(
     _RequiredListPackageVersionAssetsRequestRequestTypeDef,
     _OptionalListPackageVersionAssetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListPackageVersionDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionDependenciesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -881,63 +782,31 @@
         "domainOwner": str,
         "namespace": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListPackageVersionDependenciesRequestRequestTypeDef(
     _RequiredListPackageVersionDependenciesRequestRequestTypeDef,
     _OptionalListPackageVersionDependenciesRequestRequestTypeDef,
 ):
     pass
 
-
 PackageDependencyTypeDef = TypedDict(
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
     total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "status": PackageVersionStatusType,
-        "sortBy": Literal["PUBLISHED_TIME"],
-        "originType": PackageVersionOriginTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -953,51 +822,20 @@
         "maxResults": int,
         "nextToken": str,
         "originType": PackageVersionOriginTypeType,
     },
     total=False,
 )
 
-
 class ListPackageVersionsRequestRequestTypeDef(
     _RequiredListPackageVersionsRequestRequestTypeDef,
     _OptionalListPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-    },
-)
-_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "format": PackageFormatType,
-        "namespace": str,
-        "packagePrefix": str,
-        "publish": AllowPublishType,
-        "upstream": AllowUpstreamType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackagesRequestListPackagesPaginateTypeDef(
-    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
-    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackagesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -1012,46 +850,19 @@
         "nextToken": str,
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
     total=False,
 )
 
-
 class ListPackagesRequestRequestTypeDef(
     _RequiredListPackagesRequestRequestTypeDef, _OptionalListPackagesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "administratorAccount": str,
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
-    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesInDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
@@ -1062,45 +873,34 @@
         "repositoryPrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRepositoriesInDomainRequestRequestTypeDef(
     _RequiredListRepositoriesInDomainRequestRequestTypeDef,
     _OptionalListRepositoriesInDomainRequestRequestTypeDef,
 ):
     pass
 
-
 RepositorySummaryTypeDef = TypedDict(
     "RepositorySummaryTypeDef",
     {
         "name": str,
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
     total=False,
 )
 
-ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
-    {
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -1118,55 +918,14 @@
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
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
-_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-        "assetContent": Union[str, bytes, IO[Any], StreamingBody],
-        "assetName": str,
-        "assetSHA256": str,
-    },
-)
-_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "unfinished": bool,
-    },
-    total=False,
-)
-
-
-class PublishPackageVersionRequestRequestTypeDef(
-    _RequiredPublishPackageVersionRequestRequestTypeDef,
-    _OptionalPublishPackageVersionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredPutDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "policyDocument": str,
     },
 )
@@ -1175,22 +934,20 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
-
 class PutDomainPermissionsPolicyRequestRequestTypeDef(
     _RequiredPutDomainPermissionsPolicyRequestRequestTypeDef,
     _OptionalPutDomainPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "policyDocument": str,
     },
@@ -1200,22 +957,20 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
-
 class PutRepositoryPermissionsPolicyRequestRequestTypeDef(
     _RequiredPutRepositoryPermissionsPolicyRequestRequestTypeDef,
     _OptionalPutRepositoryPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
@@ -1226,25 +981,14 @@
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1267,83 +1011,151 @@
         "namespace": str,
         "versionRevisions": Mapping[str, str],
         "expectedStatus": PackageVersionStatusType,
     },
     total=False,
 )
 
-
 class UpdatePackageVersionsStatusRequestRequestTypeDef(
     _RequiredUpdatePackageVersionsStatusRequestRequestTypeDef,
     _OptionalUpdatePackageVersionsStatusRequestRequestTypeDef,
 ):
     pass
 
+GetAuthorizationTokenResultTypeDef = TypedDict(
+    "GetAuthorizationTokenResultTypeDef",
+    {
+        "authorizationToken": str,
+        "expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionAssetResultTypeDef = TypedDict(
+    "GetPackageVersionAssetResultTypeDef",
+    {
+        "asset": StreamingBody,
+        "assetName": str,
+        "packageVersion": str,
+        "packageVersionRevision": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionReadmeResultTypeDef = TypedDict(
+    "GetPackageVersionReadmeResultTypeDef",
+    {
+        "format": PackageFormatType,
+        "namespace": str,
+        "package": str,
+        "version": str,
+        "versionRevision": str,
+        "readme": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryEndpointResultTypeDef = TypedDict(
+    "GetRepositoryEndpointResultTypeDef",
+    {
+        "repositoryEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "assets": List[AssetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishPackageVersionResultTypeDef = TypedDict(
     "PublishPackageVersionResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+        "assetContent": BlobTypeDef,
+        "assetName": str,
+        "assetSHA256": str,
+    },
+)
+_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "unfinished": bool,
+    },
+    total=False,
+)
+
+class PublishPackageVersionRequestRequestTypeDef(
+    _RequiredPublishPackageVersionRequestRequestTypeDef,
+    _OptionalPublishPackageVersionRequestRequestTypeDef,
+):
+    pass
+
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageVersionsResultTypeDef = TypedDict(
     "DeletePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisposePackageVersionsResultTypeDef = TypedDict(
     "DisposePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageVersionsStatusResultTypeDef = TypedDict(
     "UpdatePackageVersionsStatusResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domain": str,
@@ -1354,26 +1166,24 @@
     {
         "encryptionKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
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
@@ -1381,31 +1191,31 @@
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResultTypeDef = TypedDict(
     "DescribeDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
@@ -1419,21 +1229,19 @@
         "description": str,
         "upstreams": Sequence[UpstreamRepositoryTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -1443,66 +1251,64 @@
         "domainOwner": str,
         "description": str,
         "upstreams": Sequence[UpstreamRepositoryTypeDef],
     },
     total=False,
 )
 
-
 class UpdateRepositoryRequestRequestTypeDef(
     _RequiredUpdateRepositoryRequestRequestTypeDef, _OptionalUpdateRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 DeleteDomainPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainPermissionsPolicyResultTypeDef = TypedDict(
     "GetDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "GetRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDomainPermissionsPolicyResultTypeDef = TypedDict(
     "PutDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "PutRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
@@ -1512,47 +1318,168 @@
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+    },
+)
+_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
+    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
     },
 )
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "status": PackageVersionStatusType,
+        "sortBy": Literal["PUBLISHED_TIME"],
+        "originType": PackageVersionOriginTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+    },
+)
+_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "format": PackageFormatType,
+        "namespace": str,
+        "packagePrefix": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackagesRequestListPackagesPaginateTypeDef(
+    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
+    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
+):
+    pass
+
+_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "administratorAccount": str,
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
+    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+):
+    pass
+
+ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    {
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "dependencies": List[PackageDependencyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesInDomainResultTypeDef = TypedDict(
     "ListRepositoriesInDomainResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesResultTypeDef = TypedDict(
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
         "restrictions": PackageOriginRestrictionsTypeDef,
@@ -1575,22 +1502,20 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
-
 class PutPackageOriginConfigurationRequestRequestTypeDef(
     _RequiredPutPackageOriginConfigurationRequestRequestTypeDef,
     _OptionalPutPackageOriginConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 RepositoryDescriptionTypeDef = TypedDict(
     "RepositoryDescriptionTypeDef",
     {
         "name": str,
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
@@ -1635,21 +1560,19 @@
     {
         "revision": str,
         "origin": PackageVersionOriginTypeDef,
     },
     total=False,
 )
 
-
 class PackageVersionSummaryTypeDef(
     _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
 ):
     pass
 
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
@@ -1668,104 +1591,104 @@
     total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateExternalConnectionResultTypeDef = TypedDict(
     "AssociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResultTypeDef = TypedDict(
     "CreateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResultTypeDef = TypedDict(
     "DeleteRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryResultTypeDef = TypedDict(
     "DescribeRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateExternalConnectionResultTypeDef = TypedDict(
     "DisassociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRepositoryResultTypeDef = TypedDict(
     "UpdateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageVersionResultTypeDef = TypedDict(
     "DescribePackageVersionResultTypeDef",
     {
         "packageVersion": PackageVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResultTypeDef = TypedDict(
     "ListPackageVersionsResultTypeDef",
     {
         "defaultDisplayVersion": str,
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResultTypeDef = TypedDict(
     "DeletePackageResultTypeDef",
     {
         "deletedPackage": PackageSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResultTypeDef = TypedDict(
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact/type_defs.pyi` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codeartifact.type_defs import AssetSummaryTypeDef
 
-    data: AssetSummaryTypeDef = {...}
+    data: AssetSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,17 +33,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -58,52 +61,45 @@
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
-    "GetAuthorizationTokenResultTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
-    "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
-    "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
-    "GetRepositoryEndpointResultTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
-    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PackageOriginRestrictionsTypeDef",
-    "PaginatorConfigTypeDef",
-    "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
+    "GetAuthorizationTokenResultTypeDef",
+    "GetPackageVersionAssetResultTypeDef",
+    "GetPackageVersionReadmeResultTypeDef",
+    "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
+    "PublishPackageVersionRequestRequestTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -116,14 +112,20 @@
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
@@ -155,17 +157,19 @@
     {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
     total=False,
 )
 
+
 class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
     pass
 
+
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -174,20 +178,34 @@
     "_OptionalAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class AssociateExternalConnectionRequestRequestTypeDef(
     _RequiredAssociateExternalConnectionRequestRequestTypeDef,
     _OptionalAssociateExternalConnectionRequestRequestTypeDef,
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
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -203,20 +221,22 @@
         "versionRevisions": Mapping[str, str],
         "allowOverwrite": bool,
         "includeFromUpstream": bool,
     },
     total=False,
 )
 
+
 class CopyPackageVersionsRequestRequestTypeDef(
     _RequiredCopyPackageVersionsRequestRequestTypeDef,
     _OptionalCopyPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
     total=False,
@@ -273,20 +293,22 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
+
 class DeleteDomainPermissionsPolicyRequestRequestTypeDef(
     _RequiredDeleteDomainPermissionsPolicyRequestRequestTypeDef,
     _OptionalDeleteDomainPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
@@ -303,19 +325,21 @@
     "_OptionalDeleteDomainRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class DeleteDomainRequestRequestTypeDef(
     _RequiredDeleteDomainRequestRequestTypeDef, _OptionalDeleteDomainRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -326,19 +350,21 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
+
 class DeletePackageRequestRequestTypeDef(
     _RequiredDeletePackageRequestRequestTypeDef, _OptionalDeletePackageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeletePackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -351,20 +377,22 @@
         "domainOwner": str,
         "namespace": str,
         "expectedStatus": PackageVersionStatusType,
     },
     total=False,
 )
 
+
 class DeletePackageVersionsRequestRequestTypeDef(
     _RequiredDeletePackageVersionsRequestRequestTypeDef,
     _OptionalDeletePackageVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -373,20 +401,22 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryPermissionsPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPermissionsPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -394,38 +424,42 @@
     "_OptionalDeleteRepositoryRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalDescribeDomainRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeDomainRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class DescribeDomainRequestRequestTypeDef(
     _RequiredDescribeDomainRequestRequestTypeDef, _OptionalDescribeDomainRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -436,19 +470,21 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
+
 class DescribePackageRequestRequestTypeDef(
     _RequiredDescribePackageRequestRequestTypeDef, _OptionalDescribePackageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribePackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -460,20 +496,22 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
+
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRepositoryRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -481,20 +519,22 @@
     "_OptionalDescribeRepositoryRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class DescribeRepositoryRequestRequestTypeDef(
     _RequiredDescribeRepositoryRequestRequestTypeDef,
     _OptionalDescribeRepositoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisassociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -503,20 +543,22 @@
     "_OptionalDisassociateExternalConnectionRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class DisassociateExternalConnectionRequestRequestTypeDef(
     _RequiredDisassociateExternalConnectionRequestRequestTypeDef,
     _OptionalDisassociateExternalConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisposePackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDisposePackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -530,20 +572,22 @@
         "namespace": str,
         "versionRevisions": Mapping[str, str],
         "expectedStatus": PackageVersionStatusType,
     },
     total=False,
 )
 
+
 class DisposePackageVersionsRequestRequestTypeDef(
     _RequiredDisposePackageVersionsRequestRequestTypeDef,
     _OptionalDisposePackageVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
     total=False,
@@ -573,28 +617,21 @@
     {
         "domainOwner": str,
         "durationSeconds": int,
     },
     total=False,
 )
 
+
 class GetAuthorizationTokenRequestRequestTypeDef(
     _RequiredGetAuthorizationTokenRequestRequestTypeDef,
     _OptionalGetAuthorizationTokenRequestRequestTypeDef,
 ):
     pass
 
-GetAuthorizationTokenResultTypeDef = TypedDict(
-    "GetAuthorizationTokenResultTypeDef",
-    {
-        "authorizationToken": str,
-        "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
@@ -602,20 +639,22 @@
     "_OptionalGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class GetDomainPermissionsPolicyRequestRequestTypeDef(
     _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef,
     _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetPackageVersionAssetRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionAssetRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -629,30 +668,21 @@
         "domainOwner": str,
         "namespace": str,
         "packageVersionRevision": str,
     },
     total=False,
 )
 
+
 class GetPackageVersionAssetRequestRequestTypeDef(
     _RequiredGetPackageVersionAssetRequestRequestTypeDef,
     _OptionalGetPackageVersionAssetRequestRequestTypeDef,
 ):
     pass
 
-GetPackageVersionAssetResultTypeDef = TypedDict(
-    "GetPackageVersionAssetResultTypeDef",
-    {
-        "asset": StreamingBody,
-        "assetName": str,
-        "packageVersion": str,
-        "packageVersionRevision": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetPackageVersionReadmeRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionReadmeRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
@@ -665,32 +695,21 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
+
 class GetPackageVersionReadmeRequestRequestTypeDef(
     _RequiredGetPackageVersionReadmeRequestRequestTypeDef,
     _OptionalGetPackageVersionReadmeRequestRequestTypeDef,
 ):
     pass
 
-GetPackageVersionReadmeResultTypeDef = TypedDict(
-    "GetPackageVersionReadmeResultTypeDef",
-    {
-        "format": PackageFormatType,
-        "namespace": str,
-        "package": str,
-        "version": str,
-        "versionRevision": str,
-        "readme": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetRepositoryEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
@@ -700,27 +719,21 @@
     "_OptionalGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class GetRepositoryEndpointRequestRequestTypeDef(
     _RequiredGetRepositoryEndpointRequestRequestTypeDef,
     _OptionalGetRepositoryEndpointRequestRequestTypeDef,
 ):
     pass
 
-GetRepositoryEndpointResultTypeDef = TypedDict(
-    "GetRepositoryEndpointResultTypeDef",
-    {
-        "repositoryEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
@@ -729,72 +742,50 @@
     "_OptionalGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domainOwner": str,
     },
     total=False,
 )
 
+
 class GetRepositoryPermissionsPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-    },
-)
-_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
-    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -808,20 +799,22 @@
         "namespace": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListPackageVersionAssetsRequestRequestTypeDef(
     _RequiredListPackageVersionAssetsRequestRequestTypeDef,
     _OptionalListPackageVersionAssetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListPackageVersionDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionDependenciesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -834,59 +827,33 @@
         "domainOwner": str,
         "namespace": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListPackageVersionDependenciesRequestRequestTypeDef(
     _RequiredListPackageVersionDependenciesRequestRequestTypeDef,
     _OptionalListPackageVersionDependenciesRequestRequestTypeDef,
 ):
     pass
 
+
 PackageDependencyTypeDef = TypedDict(
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
     total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "status": PackageVersionStatusType,
-        "sortBy": Literal["PUBLISHED_TIME"],
-        "originType": PackageVersionOriginTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -902,46 +869,21 @@
         "maxResults": int,
         "nextToken": str,
         "originType": PackageVersionOriginTypeType,
     },
     total=False,
 )
 
+
 class ListPackageVersionsRequestRequestTypeDef(
     _RequiredListPackageVersionsRequestRequestTypeDef,
     _OptionalListPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-    },
-)
-_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "format": PackageFormatType,
-        "namespace": str,
-        "packagePrefix": str,
-        "publish": AllowPublishType,
-        "upstream": AllowUpstreamType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackagesRequestListPackagesPaginateTypeDef(
-    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
-    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
-):
-    pass
 
 _RequiredListPackagesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
@@ -957,41 +899,20 @@
         "nextToken": str,
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
     total=False,
 )
 
+
 class ListPackagesRequestRequestTypeDef(
     _RequiredListPackagesRequestRequestTypeDef, _OptionalListPackagesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "administratorAccount": str,
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
-    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-):
-    pass
 
 _RequiredListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesInDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
@@ -1003,43 +924,36 @@
         "repositoryPrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListRepositoriesInDomainRequestRequestTypeDef(
     _RequiredListRepositoriesInDomainRequestRequestTypeDef,
     _OptionalListRepositoriesInDomainRequestRequestTypeDef,
 ):
     pass
 
+
 RepositorySummaryTypeDef = TypedDict(
     "RepositorySummaryTypeDef",
     {
         "name": str,
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
     total=False,
 )
 
-ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
-    {
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -1057,53 +971,14 @@
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
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
-_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-        "assetContent": Union[str, bytes, IO[Any], StreamingBody],
-        "assetName": str,
-        "assetSHA256": str,
-    },
-)
-_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "unfinished": bool,
-    },
-    total=False,
-)
-
-class PublishPackageVersionRequestRequestTypeDef(
-    _RequiredPublishPackageVersionRequestRequestTypeDef,
-    _OptionalPublishPackageVersionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredPutDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "policyDocument": str,
     },
 )
@@ -1112,20 +987,22 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
+
 class PutDomainPermissionsPolicyRequestRequestTypeDef(
     _RequiredPutDomainPermissionsPolicyRequestRequestTypeDef,
     _OptionalPutDomainPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "policyDocument": str,
     },
@@ -1135,20 +1012,22 @@
     {
         "domainOwner": str,
         "policyRevision": str,
     },
     total=False,
 )
 
+
 class PutRepositoryPermissionsPolicyRequestRequestTypeDef(
     _RequiredPutRepositoryPermissionsPolicyRequestRequestTypeDef,
     _OptionalPutRepositoryPermissionsPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
@@ -1159,25 +1038,14 @@
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1200,81 +1068,155 @@
         "namespace": str,
         "versionRevisions": Mapping[str, str],
         "expectedStatus": PackageVersionStatusType,
     },
     total=False,
 )
 
+
 class UpdatePackageVersionsStatusRequestRequestTypeDef(
     _RequiredUpdatePackageVersionsStatusRequestRequestTypeDef,
     _OptionalUpdatePackageVersionsStatusRequestRequestTypeDef,
 ):
     pass
 
+
+GetAuthorizationTokenResultTypeDef = TypedDict(
+    "GetAuthorizationTokenResultTypeDef",
+    {
+        "authorizationToken": str,
+        "expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionAssetResultTypeDef = TypedDict(
+    "GetPackageVersionAssetResultTypeDef",
+    {
+        "asset": StreamingBody,
+        "assetName": str,
+        "packageVersion": str,
+        "packageVersionRevision": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionReadmeResultTypeDef = TypedDict(
+    "GetPackageVersionReadmeResultTypeDef",
+    {
+        "format": PackageFormatType,
+        "namespace": str,
+        "package": str,
+        "version": str,
+        "versionRevision": str,
+        "readme": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryEndpointResultTypeDef = TypedDict(
+    "GetRepositoryEndpointResultTypeDef",
+    {
+        "repositoryEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "assets": List[AssetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishPackageVersionResultTypeDef = TypedDict(
     "PublishPackageVersionResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+        "assetContent": BlobTypeDef,
+        "assetName": str,
+        "assetSHA256": str,
     },
 )
+_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "unfinished": bool,
+    },
+    total=False,
+)
+
+
+class PublishPackageVersionRequestRequestTypeDef(
+    _RequiredPublishPackageVersionRequestRequestTypeDef,
+    _OptionalPublishPackageVersionRequestRequestTypeDef,
+):
+    pass
+
 
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageVersionsResultTypeDef = TypedDict(
     "DeletePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisposePackageVersionsResultTypeDef = TypedDict(
     "DisposePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageVersionsStatusResultTypeDef = TypedDict(
     "UpdatePackageVersionsStatusResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domain": str,
@@ -1285,24 +1227,26 @@
     {
         "encryptionKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
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
@@ -1310,31 +1254,31 @@
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResultTypeDef = TypedDict(
     "DescribeDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
@@ -1348,19 +1292,21 @@
         "description": str,
         "upstreams": Sequence[UpstreamRepositoryTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -1370,64 +1316,66 @@
         "domainOwner": str,
         "description": str,
         "upstreams": Sequence[UpstreamRepositoryTypeDef],
     },
     total=False,
 )
 
+
 class UpdateRepositoryRequestRequestTypeDef(
     _RequiredUpdateRepositoryRequestRequestTypeDef, _OptionalUpdateRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 DeleteDomainPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainPermissionsPolicyResultTypeDef = TypedDict(
     "GetDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "GetRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDomainPermissionsPolicyResultTypeDef = TypedDict(
     "PutDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "PutRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
@@ -1437,47 +1385,176 @@
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+    },
+)
+_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
+    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "status": PackageVersionStatusType,
+        "sortBy": Literal["PUBLISHED_TIME"],
+        "originType": PackageVersionOriginTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+    },
+)
+_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "format": PackageFormatType,
+        "namespace": str,
+        "packagePrefix": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackagesRequestListPackagesPaginateTypeDef(
+    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
+    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "administratorAccount": str,
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
+    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+):
+    pass
+
+
+ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    {
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "dependencies": List[PackageDependencyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesInDomainResultTypeDef = TypedDict(
     "ListRepositoriesInDomainResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesResultTypeDef = TypedDict(
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
         "restrictions": PackageOriginRestrictionsTypeDef,
@@ -1500,20 +1577,22 @@
     {
         "domainOwner": str,
         "namespace": str,
     },
     total=False,
 )
 
+
 class PutPackageOriginConfigurationRequestRequestTypeDef(
     _RequiredPutPackageOriginConfigurationRequestRequestTypeDef,
     _OptionalPutPackageOriginConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 RepositoryDescriptionTypeDef = TypedDict(
     "RepositoryDescriptionTypeDef",
     {
         "name": str,
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
@@ -1558,19 +1637,21 @@
     {
         "revision": str,
         "origin": PackageVersionOriginTypeDef,
     },
     total=False,
 )
 
+
 class PackageVersionSummaryTypeDef(
     _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
 ):
     pass
 
+
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
@@ -1589,104 +1670,104 @@
     total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateExternalConnectionResultTypeDef = TypedDict(
     "AssociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResultTypeDef = TypedDict(
     "CreateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResultTypeDef = TypedDict(
     "DeleteRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryResultTypeDef = TypedDict(
     "DescribeRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateExternalConnectionResultTypeDef = TypedDict(
     "DisassociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRepositoryResultTypeDef = TypedDict(
     "UpdateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageVersionResultTypeDef = TypedDict(
     "DescribePackageVersionResultTypeDef",
     {
         "packageVersion": PackageVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResultTypeDef = TypedDict(
     "ListPackageVersionsResultTypeDef",
     {
         "defaultDisplayVersion": str,
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResultTypeDef = TypedDict(
     "DeletePackageResultTypeDef",
     {
         "deletedPackage": PackageSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResultTypeDef = TypedDict(
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/PKG-INFO` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeartifact
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeartifact type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeartifact type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeartifact"></a>
 
 # types-aiobotocore-codeartifact
 
 [![PyPI - types-aiobotocore-codeartifact](https://img.shields.io/pypi/v/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeartifact?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeartifact)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeArtifact 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [types-aiobotocore-codeartifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/).
 
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
@@ -340,25 +339,27 @@
 )
 
 
 def check_value(value: AllowPublishType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeartifact.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -373,52 +374,45 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
-    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PackageOriginRestrictionsTypeDef,
-    PaginatorConfigTypeDef,
-    PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
+    GetPackageVersionAssetResultTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
+    PublishPackageVersionRequestRequestTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -431,14 +425,20 @@
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
@@ -456,15 +456,15 @@
     ListPackageVersionsResultTypeDef,
     DescribePackageResultTypeDef,
     DeletePackageResultTypeDef,
     ListPackagesResultTypeDef,
 )
 
 
-def get_structure() -> AssetSummaryTypeDef:
+def get_value() -> AssetSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeartifact-2.5.2/types_aiobotocore_codeartifact.egg-info/SOURCES.txt` & `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

